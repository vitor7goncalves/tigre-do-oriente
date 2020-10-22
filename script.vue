new Vue({
    el: '#app',
   
    data: {
        mobilePainel: "painelOff",
        more_: "painelOff",
        style_: "painelOff",
        event_: "painelOff",
        contact_: "painelOff",
        setArrow: [
            morArrow = "returnArrow",
            styArrow = "returnArrow",
            eveArrow = "returnArrow",
            contArrow = "returnArrow",
        ],
        showBanner: "active",
        showTitle:  "activeTitle",
        showBanner2: "inactive",
        showTitle2:  "inactiveTitle",
        showBanner3: "inactive",
        showTitle3:  "inactiveTitle",
        showBanner4: "inactive",
        showTitle4:  "inactiveTitle",
        rotate1: "activeButton",
        rotate2: "inactiveButton",
        rotate3: "inactiveButton",
        rotate4: "inactiveButton",
        clock: 1,
        subTitle: "Instrutores",
        instructors:[ 
            { name1: "Luiz Henrique da Costa"},
            { name2: "Bruno Mendes"},
            { name3: "Sonia"},
            { name4: "Frederico"},
        ],
        textInstructors:[
            {text1: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Magni repellendus ratione dicta error quod eum laudantium minima consectetur numquam blanditiis, laboriosam illum nesciunt eius alias molestias? Molestias eveniet excepturi ratione."},
            {text2: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Magni repellendus ratione dicta error quod eum laudantium minima consectetur numquam blanditiis, laboriosam illum nesciunt eius alias molestias? Molestias eveniet excepturi ratione."},
            {text3: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Magni repellendus ratione dicta error quod eum laudantium minima consectetur numquam blanditiis, laboriosam illum nesciunt eius alias molestias? Molestias eveniet excepturi ratione."},
            {text4: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Magni repellendus ratione dicta error quod eum laudantium minima consectetur numquam blanditiis, laboriosam illum nesciunt eius alias molestias? Molestias eveniet excepturi ratione."},
          
        ], 
        filosophys: "Filosofia",
        textFilo:"Lorem ipsum dolor sit amet consectetur adipisicing elit. Neque esse molestias sunt officiis eum voluptates amet impedit quia iure, aliquid laudantium sit doloremque iste quaerat at nemo culpa iusto eaque.",
        galery: "Galeria",
        warning: "Participe de uma aula grátis",
        adressTitle: "Edereço",
        adress: "Rua: Sem nome - Centro - Queimados - RJ",
           
    },
    
    methods: {
       onClick(){
          this.clock = 2;
       },

       onClick2(){
          this.clock = 8;
       },

       onClick3(){
          this.clock = 17;
       },
       onClick4(){
          this.clock = 25;
       },

       more(){
           if(this.more_ === "painelOff"){
            this.more_ = "painelOn";
            this.style_ = "painelOff";
            this.event_ = "painelOff";
            this.contact_ = "painelOff";
            this.setArrow.morArrow = "moveArrow";
            this.setArrow.styArrow = "returnArrow";
            this.setArrow.eveArrow = "returnArrow";
            this.setArrow.contArrow = "returnArrow";
           }else{
            this.more_ = "painelOff";
            this.style_ = "painelOff";
            this.event_ = "painelOff";
            this.contact_ = "painelOff";
            this.setArrow.morArrow = "returnArrow";
            this.setArrow.styArrow = "returnArrow";
            this.setArrow.eveArrow = "returnArrow";
            this.setArrow.contArrow = "returnArrow";
           }
       },
       styles(){
           if(this.style_ === "painelOff"){
            this.more_ = "painelOff";
            this.style_ = "painelOn";
            this.event_ = "painelOff";
            this.contact_ = "painelOff";
            this.setArrow.morArrow = "returnArrow";
            this.setArrow.styArrow = "moveArrow";
            this.setArrow.eveArrow = "returnArrow";
            this.setArrow.contArrow = "returnArrow";
           }else{
            this.more_ = "painelOff";
            this.style_ = "painelOff";
            this.event_ = "painelOff";
            this.contact_ = "painelOff";
            this.setArrow.morArrow = "returnArrow";
            this.setArrow.styArrow = "returnArrow";
            this.setArrow.eveArrow = "returnArrow";
            this.setArrow.contArrow = "returnArrow";
           }
       },
       events(){
           if(this.event_ === "painelOff"){
            this.more_ = "painelOff";
            this.style_ = "painelOff";
            this.event_ = "painelOn";
            this.contact_ = "painelOff";
            this.setArrow.morArrow = "returnArrow";
            this.setArrow.styArrow = "returnArrow";
            this.setArrow.eveArrow = "moveArrow";
            this.setArrow.contArrow = "returnArrow";
           }else{
            this.more_ = "painelOff";
            this.style_ = "painelOff";
            this.event_ = "painelOff";
            this.contact_ = "painelOff";
            this.setArrow.morArrow = "returnArrow";
            this.setArrow.styArrow = "returnArrow";
            this.setArrow.eveArrow = "returnArrow";
            this.setArrow.contArrow = "returnArrow";
           }
       },
       contacts(){
           if(this.contact_ === "painelOff"){
            this.more_ = "painelOff";
            this.style_ = "painelOff";
            this.event_ = "painelOff";
            this.contact_ = "painelOn";
            this.setArrow.morArrow = "returnArrow";
            this.setArrow.styArrow = "returnArrow";
            this.setArrow.eveArrow = "returnArrow";
            this.setArrow.contArrow = "moveArrow";
           }else{
            this.more_ = "painelOff";
            this.style_ = "painelOff";
            this.event_ = "painelOff";
            this.contact_ = "painelOff";
            this.setArrow.morArrow = "returnArrow";
            this.setArrow.styArrow = "returnArrow";
            this.setArrow.eveArrow = "returnArrow";
            this.setArrow.contArrow = "returnArrow";
           }
       },
       mobileSet(){
            if(this.mobilePainel === "painelOff"){
                this.mobilePainel = "painelOn";
            }
       },
       mobileSetClose(){
           this.mobilePainel = "painelOff";
       },
       
       lowTime(){
           this.clock ++;
           
                if(this.clock > 30){
                    this.clock = 0;
                }
                    if(this.clock <= 7 ){
                            this.showBanner = "active"
                            this.showTitle = "activeTitle"
                            this.showBanner2 = "inactive"
                            this.showTitle2 = "inactiveTitle"
                            this.showBanner3 = "inactive"
                            this.showTitle3 = "inactiveTitle"
                            this.showBanner4 = "inactive"
                            this.showTitle4 = "inactiveTitle"
                            this.rotate1 = "activeButton"
                            this.rotate2= "inactiveButton"
                            this.rotate3= "inactiveButton"
                            this.rotate4= "inactiveButton"
                   }else if( this.clock >= 8 && this.clock <= 15  ){
                            this.showBanner = "inactive"
                            this.showTitle = "inactiveTitle"
                            this.showBanner2 = "active"
                            this.showTitle2 = "activeTitle"
                            this.showBanner3 = "inactive"
                            this.showTitle3 = "inactiveTitle"
                            this.showBanner4 = "inactive"
                            this.showTitle4 = "inactiveTitle"
                            this.rotate1 = "inactiveButton"
                            this.rotate2= "activeButton"
                            this.rotate3= "inactiveButton"
                            this.rotate4= "inactiveButton"
                   }
                   else if( this.clock >= 16 && this.clock <= 23 ){
                            this.showBanner = "inactive"
                            this.showTitle = "inactiveTitle"
                            this.showBanner2 = "inactive"
                            this.showTitle2 = "inactiveTitle"
                            this.showBanner3 = "active"
                            this.showTitle3 = "activeTitle"
                            this.showBanner4 = "inactive"
                            this.showTitle4 = "inactiveTitle"
                            this.rotate1 = "inactiveButton"
                            this.rotate2= "inactiveButton"
                            this.rotate3= "activeButton"
                            this.rotate4= "inactiveButton"
                   }
                   else if( this.clock >= 23 ){
                            this.showBanner = "inactive"
                            this.showTitle = "inactiveTitle"
                            this.showBanner2 = "inactive"
                            this.showTitle2 = "inactiveTitle"
                            this.showBanner3 = "inactive"
                            this.showTitle3 = "inactiveTitle"
                            this.showBanner4 = "active"
                            this.showTitle4 = "activeTitle"
                            this.rotate1 = "inactiveButton"
                            this.rotate2= "inactiveButton"
                            this.rotate3= "inactiveButton"
                            this.rotate4= "activeButton"
                   }
       },
    },

    created() {
        var vm = this;
        var crono = 1000;
        
        setInterval(function(){
            vm.lowTime()
        }, crono)

    },
})
