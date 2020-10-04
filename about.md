---
layout: page
title: About
permalink: /about/
---

안녕하세요, 저는 한문희입니다.

웹 관련 디자이너 퍼블리셔 프론트앤드 개발경력이 있고

지금은 SI업무를 주로 하고있으며 웹 풀스텍 개발을 하고있습니다.

주 언어는 자바입니다.

반갑습니다.

- - -

**Skill**
<div id="chartContainer" style="height: 300px; width: 100%;"></div>

<br />

**경력**

2020.05 ~ &emsp;&emsp;&emsp;&nbsp;- 아이티키 (Web Fullstack Developer, JAVA Developer)

2018.03 ~ 2019.04 - 스튜디오 헤이데이 (Web Publisher, Web Front End Developer)

2016.11 ~ 2017.08 - 모든세븐 (Web Designer, Web Publisher)

2014.04 ~ 2016.03 - 몬스트로 (Web Designer, Web Publisher)

<br />

**교육**

2019.06 ~ 2019.12 - 비트컴퓨터학원(서초점) - 자바기반 웹 오픈소스 개발자 과정

2017.09 ~ 2017.11 - sbs아카데미학원(강남점) - Jquery, 반응형 2개월, 개인 포트폴리오 사이트 리뉴얼 1개월

2016.04 ~ 2016.08 - sbs아카데미학원(강남점) - CSS, JQUERY, 웹포트폴리오 제작

<br />

**프로젝트**

2020.09~ &emsp;&emsp;&emsp;&nbsp;KAC(코리아오토글라스) ERP 시스템 구축 - [ORACLE, JAVA, SPRING, JAVASCRIPT, WebSquare, Jquery, SVN]

2020.06~2020.08 NAVER LINE BANK 대만 웹사이트 개발 및 품질관리 - [ORACLE, JAVA, SPRING, JAVASCRIPT, GIT, ZIRA]

2019.11~2019.12 MINT 쇼핑몰 프로젝트(포트폴리오) - [Oracle, Java, Spring, Javascript]

2019.08~2019.09 일본제품 불매 및 친일청산 범국민 서명운동 웹프로그램 사이트 - [MySql, Php, Javascript]

2018.07~2019.02 삼성생명 FDP 프로젝트 - [Html5, Css3, VueJS, GIT]

2018.03~2018.06 한샘 몰 유지보수, 기획전 프런트 개발 - [JAVA, SPRING, Html5, Css3, Javascript, Jquery, SVN]

2017.01~2017.08 종로학원 8개 지점 유지보수 - [PhotoShop, Html5, Css3]

<br />

**email: mun01180@gmail.com**

<!-- ABOUT SKILL : START -->
<script>
window.onload = function() {

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
        { y: 80, label: "80%", indexLabel: "Git / SVN" },
        { y: 60, label: "60%", indexLabel: "SQL / MYSQL" },
        { y: 60, label: "60%", indexLabel: "Spring" },
        { y: 70, label: "70%", indexLabel: "JAVA" },
        { y: 70, label: "70%", indexLabel: "AJAX" },
        { y: 70, label: "70%", indexLabel: "WebSquare" },
        { y: 70, label: "70%", indexLabel: "Javascript / ECMA6" },
        { y: 90, label: "90%", indexLabel: "HTML / CSS / MediaQuery" }
      ]
    }]
  };

  $("#chartContainer").CanvasJSChart(options);
  $(".canvasjs-chart-credit").css("display", "none");
}

</script>
<!-- ABOUT SKILL : END -->
