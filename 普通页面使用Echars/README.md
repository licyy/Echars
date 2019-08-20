2019/8/20
    创建简单Echars实例

        将Echars图形绑定到dom
        var myChart = echarts.init(document.getElementById("main"))

        指定图表的配置文件和数据
        option={
            title:{},    <!-- 标题-->
            tooltip:{},    <!-- 提示框 -->  
            legend:{        <!-- 创建一个图例 --> 
                data: ['销量']
            },
            xAxis:{         <!-- x轴显示数据 --> 
                data: ["衬衫", "羊毛衫", "雪纺衫", "裤子", "高跟鞋", "袜子"]
            },
            yAxis: { },   <!-- y轴显示数据 --> 
            series: [{      <!-- 指定系列 --> 
                name: "销量",   
                type: "bar",    <!-- 指定为柱状图系列 -->
                data: [5, 30, 10, 20, 10, 36]   <!--具体数据-->
            }]  
        }

        将配置项和数据绑定到dom上
        myChart.setOption(option)



