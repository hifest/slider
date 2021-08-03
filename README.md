# slider

### you can write properties in any order

# properties:
| properties | method|
| ------------- |:-------------:|
| Container       | the container containing the slider and its slides|
| nextArrow      | an arrow that will flip the slider to the left (or the next slide) | 
| prevArrow      |arrow that will flip the slider to the right (or the previous slide)     | 
|  wrapper | wrapper that has a slider (slides only)      |
| totalCounter | the id of the element in which the total number of slides will be written    |
| currentCounter | the id of the element in which the number of the element on which the user stopped will be written  |
| slide |  slide class  |
| field |  skider wrapper  |


### example: 

```javascript
        slider({
                container:'.offer__slider',
                nextArrow:'.offer__slider-next',
                prevArrow:'.offer__slider-prev',
                wrapper: '.offer__slider-wrapper',
                totalCounter: '#total',
                currentCounter: '#current',
                slide:'.offer__slide',
                field:'.offer__slider-inner'
        });

```

### download this file sliderFull.min.css if you will use the layout as shown in the example

### example layout:
 
 ``` HTML
  <div class="offer__advantages">
                <h2>Быстро и полезно</h2>
                <div class="offer__advantages-text">
                    Готовка дома занимает много сил, времени и нервов. Мы привозим еду сразу на целый день, и ты можешь действовать так, как тебе удобно, не подстраиваясь ни под кого и будучи уверенным в качестве продукта!
                </div>
                <h2>Правильный рацион</h2>
                <div class="offer__advantages-text">
                    Мы разработали специальное меню, где учтены все нюансы правильного питания, от баланса БЖУ до их приготовления и дробления рациона.
                </div>
            </div>
            <div class="offer__slider"> //container
                <div class="offer__slider-counter">
                    <div class="offer__slider-prev">
                        <img src="icons/left.svg" alt="prev"> //prevArrow
                    </div>
                    <span id="current">03</span> / ///currentCounter
                    <span id="total"></span>//totalCounter
                    <div class="offer__slider-next"> //nextArrow
                        <img src="icons/right.svg" alt="next">
                    </div>
                </div>
                <div class="offer__slider-wrapper">//wrapper
                    <div class="offer__slider-inner">//field
                        <div class="offer__slide">//slide
                            <img src="img/slider/pepper.jpg" alt="pepper">
                        </div>
                        <div class="offer__slide"> //slide
                            <img src="img/slider/food-12.jpg" alt="food">
                        </div>
                        <div class="offer__slide">//slide
                            <img src="img/slider/olive-oil.jpg" alt="oil">
                        </div>
                        <div class="offer__slide">//slide
                            <img src="img/slider/paprika.jpg" alt="paprika">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
 
 ```
 
 ### if you have a project collector then export the file like this:
 the file script.min.js and script.js spells out the exports, but import them into a file that collects the entire project:
 ```javascript
        import  modal from './modules/modal';  // './modules/modal' -src in which the slider file lies
 ```
