---
title: My trip to London
---
I **absolutly** wanted to visit the **UK** with my wife, especially **London** because it's the capital of the England.  
To travel there, we took the train called **Eurostar**, in a few hours we were there for the first time!  

I was so **impressed** to be in London, this was my dream. When I took the **underground**, I was completely lost because it's totally different from the Paris' one.  
On the way to my hotel, I've noticed some **red telephone boxes**. This made me laugh because it's a well-known stereotype. For my first days, I've made many English mistakes. The British accent is very particular.  

![Red Telephone Box](/img/PHONE_BOX.jpg "Red Telephone Box")<center><small><i class="img-caption">Red Telephone Box</i></small></center>

The second day. I was eager about walking on the **Tower Bridge** which is located over the **River Thames**. This was very impressive. Then I ate in a small restaurant, I ordered a typical British launch: A **Fish & Chips**.  

I also wanted to see the **Changing of the Royal Guards** at the Buckingham Palace (a must-see!). There were many tourists watching the show.  

![Buckingham](/img/BUCKINGHAM.jpg "Buckingham")<center><small><i class="img-caption">Buckingham</i></small></center>

In the evening, I took a red double decker bus to go to the **Piccadelly Circus**.  

![Double-Decker Bus](/img/redBus.jpg "Double-Decker Bus")<center><small><i class="img-caption">Double-Decker Bus</i></small></center>

![Piccadilly](/img/PICADELLY.jpg "Piccadilly")<center><small><i class="img-caption">Picadelly Circus</i></small></center>


It’s a place with a fountain in the center, and many popular shops (like Burger King®…). At the same time I saw Big Ben with the bells ringing. Then I went back to my hotel, exhausted, I turned on the TV and watched the BBC.  

The next day, it was already Sunday, I ate a traditional brunch with scrambled eggs, bacon, meat, potatoes…  
Then, **Shopping Time!** I promised to my wife, that we’ll go shopping one day! And there it is...  
We firstly went to the most popular and luxury department store: **Harrods**. It’s a big store with many articles for wealthy people. Then we wanted to make a present to our children as a British souvenir, because they are currently at my parents’ house.  

![Harrods](/img/HARRODS.jpg "Harrods")<center><small><i class="img-caption">Harrods</i></small></center>

We also went to **Hamleys** a very famous toys shop of London. There, the vendors are very kind and welcoming! The shop is extremely huge with many flours.  
Right after my wife ruined me, we went back at the hotel.  

The last day, we got up earlier so we could go to the **London Eye**.  

![London Eye](/img/LONDON_EYE.jpg "London Eye")<center><small><i class="img-caption">London Eye</i></small></center>

We took a ride on the giant wheel to admire the whole city from a high-angle! Once the ride over, we went to the **Tower of London**.  

![Tower of London](/img/Tower_of_london.jpg "Tower Of London")<center><small><i class="img-caption">Tower of London</i></small></center>  

This is an old fortress located along the River Thames. It serves as a shelter for the **Crown Jewels**.  

![Crown Jewels](/img/CROWN_JEWELS.jpg "Crown Jewels")<center><small><i class="img-caption">Crown Jewels</i></small></center>  

The jewels were gorgeous!  

Then, we finally went back to the hotel and packed our things. A taxi took us to the **London Pancras International** station to come back home in France! We found this trip extraordinary and we will, **without a doubt**, do it again with our children this time!  

<small><i>Written by Aurélien PETIT & Aurèle OULES.</i></small>  

<div id='rateform' style="margin-top: 50px">
	<input id='rate' style="text-align: center; width: 100%; margin-bottom: 10px" type="number" class="form-control" placeholder="20/20" min="0" max="20" />
	<input id='submitBtn' type="submit" style="width: 100%; margin-bottom: 10px" class="btn btn-primary" value="Rate" onclick="sendgrade()">
</div>

<script>
    function sendgrade() {
        console.log($('#rate').val());
        $.ajax({
            url: 'http://aureledocs.oules.com/aureleoules/rate.php',
            type: 'POST',
            data: {
                grade: $('#rate').val()
            },
            success: function(msg) {
                $("#rateform").append("<center><p>Grade sent.</p></center>");
                $('#submitBtn').prop('disabled', true);
                $('#rate').prop('disabled', true);
                $('#submitBtn').removeClass("btn-primary");
                console.log('success');
            },
            error: function(err) {
                console.log(err);
            }
        });
    }
</script>
