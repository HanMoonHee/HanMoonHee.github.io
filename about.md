---
layout: page
title: About
permalink: /about/
---

안녕하세요, 저는 한문희입니다.

디자인을 좋아하고 퍼블리싱업무를 주로 했었습니다.

기본적인 수준의 프론트개발 경험이 있습니다.

지금은 자바언어를 위주로 공부중입니다.

스포츠를 좋아하고 산책을 좋아합니다.

요즘은 블로그를 만들고 나만의 컨텐츠를 만들고 공부하며 개발하는것에 흥미가 생겼습니다.

반갑습니다.

----

**Skill**
<div id="chartContainer" style="height: 300px; width: 100%;"></div>

<br />

**경력**

2018.03 ~ 2019.04 - 스튜디오 헤이데이 (Web Publish, Web Front End Develop)

2016.11 ~ 2017.08 - 모든세븐 (Web Design, Web Publish)

2014.04 ~ 2016.03 - 몬스트로 (Web Design, Web Publish)

<br />

**교육**

2019.06 ~ 2019.12 - 비트컴퓨터학원(서초점) - 자바기반 웹 오픈소스 개발자 과정

2017.09 ~ 2017.11 - sbs아카데미학원(강남점) - Jquery, 반응형 2개월, 개인 포트폴리오 사이트 리뉴얼 1개월

2016.04 ~ 2016.08 - sbs아카데미학원(강남점) - CSS, JQUERY, 웹포트폴리오 제작

<br />

**프로젝트**

2019.11~2019.12 MINT 쇼핑몰 프로젝트(포트폴리오)

2019.08~2019.09 일본제품 불매 및 친일청산 범국민 서명운동 웹프로그램 사이트

2018.07~2019.02 삼성생명 FDP 프로젝트

2018.03~2018.06 한샘 몰 유지보수, 기획전 프런트 개발

2017.01~2017.08 종로학원 8개 지점 유지보수

<br />

**email: mun01180@gmail.com**

<script>
window.onload = function () {

var options = {
	animationEnabled: true,
	title: {
		text: "",                
		fontColor: "Peru"
	},
	axisY: {
		tickThickness: 0,
		lineThickness: 0,
		valueFormatString: " ",
		gridThickness: 0                    
	},
	axisX: {
		tickThickness: 0,
		lineThickness: 0,
		labelFontSize: 18,
		labelFontColor: "Peru"				
	},
	data: [{
		indexLabelFontSize: 14,
		toolTipContent: "<span style=\"color:#62C9C3\">{indexLabel}:</span> <span style=\"color:#CD853F\"><strong>{y}</strong></span>",
		indexLabelPlacement: "inside",
		indexLabelFontColor: "white",
		indexLabelFontWeight: 400,
		indexLabelFontFamily: "Verdana",
		color: "#62C9C3",
		type: "bar",
		dataPoints: [
			{ y: 60, label: "60%", indexLabel: "Git / Github" },
			{ y: 30, label: "30%", indexLabel: "SQL / MYSQL" },
			{ y: 55, label: "55%", indexLabel: "Spring / Jsp" },
			{ y: 40, label: "40%", indexLabel: "JAVA" },
			{ y: 70, label: "70%", indexLabel: "AJAX" },
			{ y: 40, label: "40%", indexLabel: "Vue" },
			{ y: 70, label: "70%", indexLabel: "Jquery" },
			{ y: 50, label: "50%", indexLabel: "Javascript / ECMA6" },
			{ y: 90, label: "90%", indexLabel: "HTML / CSS / MediaQuery" }
		]
	}]
};

$("#chartContainer").CanvasJSChart(options);
$(".canvasjs-chart-credit").css("display", "none");

}
</script>
