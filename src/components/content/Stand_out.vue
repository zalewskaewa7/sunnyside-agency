<template>
    <div class="StandOutComponent">
        <img class="standOutImg" alt="glass" src="../../images/desktop/image-stand-out.jpg" />

        <div class="standOutText">
            <h2> Stand out to the right audience</h2>
            <p>Using a collaborative formula of designers, researchers, photographers, videographers, and copywriters, we’ll build and extend your brand in digital places. </p>
        <span>Learn more</span>
        
    </div>
    
    </div>
    </template>
    <style lang="scss">
    .StandOutComponent{
        display:flex;
        flex: 1 100%;
        flex-flow: row wrap;
        justify-content:center;
    
    
        .standOutText{
        display:flex;
        flex-flow: row wrap;
        align-items: center;
        flex: 0 40%;
        padding: 5%;
        width: 40%;
        line-height: 1.5;
    
            h2{
                padding:5%;
                font-family: "Fraunces";
                color: hsl(212, 27%, 19%);
                font-size: 3rem;
            }
            p{
                padding:5%;
                color: hsl(232, 10%, 55%);
                font-size: 1.2rem;
                font-weight: 600;
            }

            
            span{
                margin:5%;
                color: hsl(212, 27%, 19%);
                text-transform: uppercase;
                font-family: "Barlow";
                font-size: 1.1rem;
                border-radius: 8px;
                height: 8px;
                width: 115px;
                box-shadow: -5px 18px 0 0 hsl(7, 99%, 70%, 0.3);               
            }
            span:hover{
                cursor: pointer;
                box-shadow: -5px 18px 0 0 hsl(7, 99%, 70%);               

            }
            
    
        }
        .standOutImg{
            flex: 0 50%;
            width: 50%;
            height: auto;
        }
    }

    @media all and (max-width:  375px)  {

        .StandOutComponent{
            .standOutImg{
                flex: 1 100%;
                order:1;
                width: 70%;
            }
            .standOutText{
                flex: 1 100;
                justify-content: center;
                order: 2;

                h2{
                font-size: 2rem;
                text-align: center;

            }
            p{
                font-size: 1rem;
                text-align: center;

            }

            
            span{
                text-align: center;
                font-size: 1rem;

       
            }

            }


        }
    }

    
    </style>