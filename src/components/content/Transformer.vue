<template>
    <div class="transformerComponent">
    <div class="transformText">
        <h2> Transform your brand</h2>
        <p>We are a full-service creative agency specializing in helping brands grow fast. 
      Engage your clients through compelling visuals that do most of the marketing for you.</p>
        <span>Learn more</span>
    </div>
    <img class="transformImg" alt="egg" src="../../images/desktop/image-transform.jpg" />
    </div>
    </template>
    <style lang="scss">
    .transformerComponent{
        display:flex;
        flex-flow: row wrap;
        justify-content:center;
    
    
        .transformText{
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
                box-shadow: -5px 18px 0 0 hsl(51, 100%, 49%, 0.3);               
            }

            span:hover{
                cursor: pointer;
                box-shadow: -5px 18px 0 0 hsl(51, 100%, 49%);               

            }
    
        }               
        .transformImg{
            flex: 0 50%;
            width: 50%;
            height: auto;
        }
    }

    @media all and (max-width:  375px)  {
        .transformerComponent{
            
            .transformImg{
            flex: 1 100%;
            order: 1;
            width: 50%;
            height: auto;
        }
        .transformText{
        order: 2;
        flex: 1 100%;
        justify-content: center;

            h2{
                font-size: 2rem;
                text-align: center;

            }
            p{
                font-size: 1rem;
                text-align: center;

            }
            span{
                font-size: 1rem;

            }
        }
        }

    }
    
    </style>