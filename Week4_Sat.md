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

> I actually observed a perfect use for "User-select:none" as I am able to select "message." While this is small, this is a prime example of the usecase that I would deploy that utility.
>
> I do really like the fact that there is essentially "no more CSS" and that the amount to be read is much less. I could see this being an issue if someone has never used TailWind and is unfamiliar with this way
> of styling, that would be the only issue that I can think of. While readability is constantly a concern, this would be the biggest issue; however, isn't css a readability issue anyways? I like it!
>
> * input class="placeholder:italic placeholder:text-slate-400 block bg-white w-full border border-slate-300 rounded-md py-2 pl-9 pr-3 shadow-sm focus:outline-none focus:border-sky-500 focus:ring-sky-500 focus:ring-1 sm:text-sm" placeholder="Search for anything..." type="text" name="search"/>  
>
>   This was interesting. I knew this before, but have forgotten it!
>
> * div class="text-center sm:text-left"> /div>  
>   For me, I do need to play with this a little bit more in Playground as my understanding of this does seem like I understand it, but using it will help a lot. Is there a good way to actually test this? As it is tied to screen size, how would I go about testing these features easily?

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

## Flex-Grow / Flex-Shrink ##

div class="flex ...">  
   div class="flex-none w-14 h-14 ...">  
    01  
   /div>  
  div class="shrink w-64 h-14 ...">  
    02  
  /div>  
  div class="flex-none w-14 h-14 ...">  
    03  
  /div>  
/div>
> I could see myself using this to allow an image to only shrink, or grow a set amount, to eliminate the possibility of an image becoming super pixelated on a large viewport. For example, our company website, YPS-USA.com, elimates one of the images towards the top of
> the page if you shrink the viewport enough. While this is definitely an out-of-the-norm situation, we would want to account for the possibility. It would be much more beneficial for these objects to shrink, allowing for all of the objects to remain visible, to some
> extent.
>
> Sidenote: I accidentally found out that (###### XYZ ######) is the same as (###### XYZ #), kinda cool!

## Grid Column Start / End ##
div class="grid grid-cols-3 gap-4">  
  div class="...">01</div>  
  div class="...">02</div>  
  div class="...">03</div>  
  div class="col-span-2 ...">04</div>  
  div class="...">05</div>  
  div class="...">06</div>  
  div class="col-span-2 ...">07</div>  
/div>
> I did completely forget to commit often and lost a large portion of my work, so I get to learn twice!
>
> I could see myself using this tool to create a variation in a group of information. While keeping the information together in a section, yet separated by the difference in the design, would allow for users to not get lost in one large group of information.
> In my work, we struggle to get users to read inportant information, despite sending it directly to them after purchasing an item. I believe that this would allow us to "trick" their minds into actually reading a majority of the content, while keeping the content the
> same, just changing the layout from a simple left to right, top to bottom.


## Text Decoration ##
> This would essentially be useful for the same application that I previously mentioned! If I were to underline key component of information, in conjunction with the above code, this would allow users to locate a section by a specific color. Topic A could be color x;
> Topic B could be color y. This would again separate the information, allow for the ability to easily navigate, and keep the content the same! Also, the hover utility would allow us to change hyperlinks to company colors, rather than a default blue, a slight touch
> yet a personal one!

## bg Attachment ##
div class="bg-fixed ..." style="background-image: url(...)"> /div>
> I would see this being used to keep the background image in the same place to ensure that information that you want to relay to the consumer be relayed. If a phone number, busines name, or other key information is listed somewhere, you can ensure that the information
> stays in their view, regardless of where they scroll.

## Blur ##
> I had no idea that you could simply blur the image without actually editting the image! This is pretty cool, and also somewhat amusing that the differences are designated much like shirt sizes. I could see myself using this to keep the same background image for
> continuity purposes, yet bluring the image so that focus can be brought to whatever other content I would like to be noticed, especially if the background image is somewhat "busy." Backdrop Blur would be equally as useful, for the same reasons already listed.

## pointer-events ##
> I almost did not notice the difference between "pointer-events-auto" and "pointer-events-none." However, I did notice the differece, being the cursor returns to normal when outside of the actual text entry area. This is a small, yet personal, touch that would be
> noticed if "pointer-events-none" were set. I am sure I would think that the "pointer-events-none" would look janky if it were in use in the example given.

## SVG ##
> I had no idea that these were not images! Heroicons.com is now bookmarked for future use! This looks like it could make a page appear much more modern. Rather than a simple "Share" button, an SVG could be used in conjunction to make the page seem a little more
> professional. This is probably my favorite find of this assignment!

## Resize ##
> I have actually used this before, as we created a database for work that has a text entry area, which is resizeable. I will probably go back and use the User-Select utility, select all, to make it only select all of the text in said textbox. There has never been a
> time where we have needed to select only a portion on the text, so this reminded me of that!

## Caret Color ##
> Kind of nit-picky, but I could see myself using this for a contact form for our company website to include the company colors. This would be a small, yet noticeable touch. I added this to the list of things to do at work on Monday!

# General Notes #
> I did really like this website! Whether it be the Playground, Heroicons, or some of the small features that make a webpage standout from others, the examples were really good, readable, and I liked the fact that it displays the class and properties at the top of the
> page, allowing for much better understanding! Simple things like:
>
> button class="transition ease-in-out delay-150 bg-blue-500 hover:-translate-y-1 hover:scale-110 hover:bg-indigo-500 duration-300 ...">  
>  Save Changes  
> /button>  
>
> are interesting ways to add small touches to regularly used functions on a page. I also liked looking over the rotate section, as I often have a hard time visualizing from the podcast. I cannot see myself using that function for anything at this time, but I am sure
> that there is something that I am over looking that I could use this function for! Is there a way to include code in this file without removing the "<" like I had to do? I will look into that more, but I could not figure it out.
