# [Counter Project vinilla  Javascript](https://kamrulcoder.github.io/counter-project-vinilla-js/)

## This projct is very straightforward  and simple. but i can  learn something  through this project. 

### Thats what I  am learning new javascript sysntax and code here ...............

1. **ClassList contains** 
1. **Foreach Loop**

<br> 

>
> Project Code Here 

#### Html Code Here .....

```
    <div class="contianer">
        <div class="row">
            <div class="col-lg-6  offset-lg-3">
                <div class="couter-box  shadow-lg  text-center"   style="background: #B5966A; padding: 30px; margin: 100px 0;">
                    <h2 class="display-4  font-weight-bold">Counter Project </h2>
                    <div class="text-center">
                        <span class="count  display-2"  >0</span>
                    </div>
                   
                    <div class="btns  d-flex justify-content-between">
                        <button  class="btn btn-danger  lower ">Lower Count </button>
                        <button  class="btn btn-success upper ">Upper  Count </button>
                    </div>
                </div>
                
            </div>
        </div>
    </div>

```

### Javascript Code Here ........

```
  let btn = document.querySelectorAll(".btn");
        let counttext = document.querySelector(".count");
        console.log(btn)
        let count = 0

        btn.forEach(buttons => {
            buttons.addEventListener("click", function(){
               
            if(buttons.classList.contains("lower")){
                count--
            }else if ( buttons.classList.contains("upper")){
                count++;
            }
            counttext.textContent = count

            if(count > 0){
                counttext.style.color = "green"
            }else if (count  < 0 ){
                counttext.style.color = "red"
            }else{
                counttext.style.color = "black"
            }
            })          
        });
        ```
