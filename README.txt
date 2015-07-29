Please help me understand better your comments and give me solutions as well instead just feedback, something I could read that would make me understand your point or an example that would work in my case.


HTML
1) Structure

>>>>> FEEDBACK I GOT
As the previous reviewer mentioned, even though you meet the specification , you could make your grid much better.

I will give you a boilerplate code for how your grid should be structured and then point out the errors :

<body>
   <div class="container">
      <!--Row for logo and name-->
      <div class="row">
          <div class="col-md-6">
          </div>
          <div class="col-md-6">
          </div>
      </div>
     <!--Row for banner-->
      <div class="row">
         <div class="col-md-12">
         </div>
     </div>
     <!--Row for featured work-->
      <div class="row">
          <div class="col-md-4">
          </div>
          <div class="col-md-4">
          </div>
          <div class="col-md-4">
          </div>      
       </div>
   </div>
</body>

Also you will find this article helpful regarding how to lay out the grid using bootstrap :)


>>>>> WHAT I DO?
The design I’ve created concentrate in the center content but there is a background in situations like Banner and Services, I used the container inside the row exactly to be able to create this background easily. If there is another way to do it, please let me know. I went to check how Bootstrap does it for his own documentation http://getbootstrap.com/components and you can see the purple banner being created exactly the same way. :(