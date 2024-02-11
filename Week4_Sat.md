# CSS Units #

## Rem's 'n Em's ##

* Rem - Root EM, relative to root element
* em - relative to nearest parent EM (1.5em would be 1.5x bigger than the parent)
* If you set a font size to 2em or 2rem, they will be two times the size of something it is relative to
* em is based on parent that has a parent with a font size set, 
* rem is based on the root, HTML element. If fontsize is set to 10px, 2rem would be 20px.
* Might want to use em in cases where size is dependant on container
* Might want to use rems in cases where size needs to be relevant to overall document
* If you have 4 different elements in a container, you can scale them all
* HTML font size 62.5% makes 1rem=10px.
* If using em's/rem's, if you change base font, it is easily scalable
* If using px, it is relative to what _px would be based on the display being used
* Can also manually set it to 10px, but it will not take user font customization into consideration

## Viewport Units ##

* Allows you to scale based off of height x width or min/max

## CH Units ##

* 1 CH is relative to size of a "0" in font size
* only works well in a mono-size font style
* apparently not that useful (per podcast hosts)

## Percentages ##

* could be used to make <div></div> x% of container

## Flexbox ##

* flex-grow:1 - All flex items will have an equal chance to grow
* flex-grow:2 - This item will take up 2/3rd of the space if the others are set to flex-grow:1
* flex-shrink:1 - All flex items will have an equal chance to shrink
* flex-shrink:2 - This item will shrink twice as much if the others are set to flex-shrink:1

# Tailwind CSS #

## Z-Index ##
> div class="z-40 ...">05</div>  
div class="z-30 ...">04</div>  
div class="z-20 ...">03</div>  
div class="z-10 ...">02</div>  
div class="z-0 ...">01</div>  
* Covers 3D positioning
* z-40 would be placed higher on the 3D plane than z-30
* to only apply when hovering, do:  
div class="z-0 hover:z-50">  
/div>

