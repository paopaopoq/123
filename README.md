function setup() {
  createCanvas(windowWidth, windowHeight);
}

function draw() {
  background("#FFEEDD");
  noFill()
  stroke("#EA7500")  //線條顏色
  strokeWeight(1)   //線條粗細
 
  //=========宣告變數
  var rect_width = 50
  var bc_w = 50
  var sc_w = 25
  
  
  //=============================================
  //ellipse(25+bc_w*0,25,bc_w)  //畫橢圓(正圓)
  //rect(rect_width*0,0,rect_width)  //畫方形
  //ellipse(rect_width*1,50,sc_w )
  //=============================================
  //ellipse(25+bc_w*1,25,bc_w)  //畫橢圓(正圓)
 // rect(rect_width*1,0,rect_width)  //畫方形
  //ellipse(rect_width*2,50,sc_w )
  //=============================================
 // ellipse(25+bc_w*2,25,bc_w)  //畫橢圓(正圓)
 // rect(rect_width*2,0,rect_width)  //畫方形
  //ellipse(rect_width*3,50,sc_w )
  //=============================================
  //ellipse(25+bc_w*3,25,bc_w)
  //rect(rect_width*3,0,rect_width)
  //ellipse(rect_width*4,50,sc_w )
  //===================重複相同指令的for指令=======================
  rectMode(CENTER)
  //第一排
  for(let x=0;x<width;x=x+rect_width){
    ellipse(x,25+50*0,bc_w)
    rect(x,25+50*0,rect_width)
    ellipse(25+x+rect_width,50+50*0,sc_w )  
  }

  //第二排
  for(let x=0;x<width;x=x+rect_width){
    ellipse(x,25+50*1,bc_w)
    rect(x,25+50*1,rect_width)
    ellipse(25+x+rect_width,50+50*1,sc_w )  
  }

  //======================使用迴圈，產生30排==========================
  for(let j=0;j<25;j=j+1){
    for(let x=0;x<width;x=x+rect_width){
      ellipse(x,25+50*j,bc_w)
      rect(x,25+50*j,rect_width)
      ellipse(25+x+rect_width,50+50*j,sc_w )
    }

  }

}
