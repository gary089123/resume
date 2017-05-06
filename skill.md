<canvas id="myChart" width="400" height="400"></canvas>
<script>
var ctx = document.getElementById("myChart");

var data = {
    labels: ["Java", "C/C++", "Ruby", "PHP", "Web 前端", "git" ,"Linux系統"],
    datasets: [
        {
            label: "目前自我評分",
            backgroundColor: "rgba(179,181,198,0.2)",
            borderColor: "rgba(179,181,198,1)",
            pointBackgroundColor: "rgba(179,181,198,1)",
            pointBorderColor: "#fff",
            pointHoverBackgroundColor: "#fff",
            pointHoverBorderColor: "rgba(179,181,198,1)",
            data: [ 60, 55, 85, 70, 65 , 85 ,70]
        },
        {
            label: "短期學習目標",
            backgroundColor: "rgba(255,99,132,0.2)",
            borderColor: "rgba(255,99,132,1)",
            pointBackgroundColor: "rgba(255,99,132,1)",
            pointBorderColor: "#fff",
            pointHoverBackgroundColor: "#fff",
            pointHoverBorderColor: "rgba(255,99,132,1)",
            data: [65, 70, 85, 70, 75, 90, 85]
        }
    ]
};

var myRadarChart = new Chart(ctx, {
    type: 'radar',
    data: data,
    options: {
            scale: {
                reverse: true,
                ticks: {
                    beginAtZero: true
                }
            }
    }
});


</script>
