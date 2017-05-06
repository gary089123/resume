Java 具有小專案開發經驗&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;C/C++ 具有程式開發基礎&nbsp;&nbsp;&nbsp;&nbsp;Ruby 具有專案開發經驗<br>PHP 具有管理專案經驗&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Git 熟悉且專案上運用&nbsp;&nbsp;&nbsp;&nbsp;Linux管理伺服器經案
<canvas id="myChart" width="300" height="300"></canvas>
<script>
var ctx = document.getElementById("myChart");

var data = {
    labels: ["Java", "C/C++", "Ruby", "PHP", "Web 前端", "Git" ,"Linux系統"],
    datasets: [
        {
            label: "目前自我評分",
            backgroundColor: "rgba(179,181,198,0.2)",
            borderColor: "rgba(179,181,198,1)",
            pointBackgroundColor: "rgba(179,181,198,1)",
            pointBorderColor: "#fff",
            pointHoverBackgroundColor: "#fff",
            pointHoverBorderColor: "rgba(179,181,198,1)",
            data: [ 60, 55, 85, 60, 55 , 85 ,70]
        },
        {
            label: "短期學習目標",
            backgroundColor: "rgba(255,99,132,0.2)",
            borderColor: "rgba(255,99,132,1)",
            pointBackgroundColor: "rgba(255,99,132,1)",
            pointBorderColor: "#fff",
            pointHoverBackgroundColor: "#fff",
            pointHoverBorderColor: "rgba(255,99,132,1)",
            data: [65, 80, 85, 65, 70, 90, 80]
        }
    ]
};

var myRadarChart = new Chart(ctx, {
    type: 'radar',
    data: data,
    options: {
            scale: {
                ticks: {
                    beginAtZero: true,
                    max: 100
                }
            }
    }
});


</script>
