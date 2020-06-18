<script>
  import Tailwindcss from "./Tailwindcss.svelte";

  // Icon imports will be needed in your components
  import Icon from 'svelte-awesome';
  import { faThumbsUp, faThumbsDown } from '@fortawesome/free-regular-svg-icons';
  import { beer, refresh, comment, codeFork, camera, ban } from 'svelte-awesome/icons';

</script>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  h3 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 3em;
    text-align: center;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
   
  }

  @media (max-width: 640px) {
    h1{
      font-size: 3em;
    }
   
  }
 
  
</style>
<!-- The Tailwind component directly below should be imported into all
    your components that use tailwind-->
<Tailwindcss />


<main>
  <h1>Component Practice!</h1>
  <p class="px-24"> 1) In App.svelte you have a series of commented out components. It your job to 
  build the components such that App.svelte works with them uncommented, and they 
  look like vuetify ones.
  <br><br>
  
  2) For icons refer to <a href="https://github.com/RobBrazier/svelte-awesome">svelte-awesome</a>
   <Icon data={faThumbsUp}/>. Youll need to import icons into your components like at the top
   of this file.<br><br>

  3) Refer to <a href="https://vuetifyjs.com/en/components/api-explorer/">
  Vuetify</a> componets for design. Try to replicate. <br><br>

  
   
  4) Dont alter App.svelte. <br><br>
  
  5) Use tailwind. <br><br>
   
  6) Have fun! <Icon data={beer}/>
   </p>
  
</main>


<!-- Here are some button declarations that your components
    should be able to satisfy.
    
    1) All buttons should have ripple effect when clicked
    
    3) btnText attribute is where the button's text goes-->

<h3>Buttons</h3>
<section class="mx-10 my-10 ">


<!-- 
 <Button 
  btnText="Large Primary"
  color="primary"
  size="xl"
  elevation="sm"
 /> -->

<!-- Buttons can have different levels of elevation -->

 <!-- <Button 
  btnText="Block Secondary Raised High"
  color="secondary"
  size="block"
  elevation="lg"
 /> -->

 <!--default color should be purple like vuetify buttons
      default size is md-->

 <!-- <Button
  btnText="Rounded"
  rounded={true} /> -->

 <!-- <Button 
  btnText="Outline"
  outline={true} /> -->

 <!-- <Button 
  btnText="Text Button"
  textMode={true} /> -->

<!-- by default disabled is false. Buttons should be disableable-->
 
 <!-- <Button
  btnText="Disabled"
  disabled={true} /> -->

<!-- put an icon in this button. No btnText-->

 <!-- <Button fab={true} 
    elevation="lg"
    iconData={comment}/> -->

    <!-- <Button fab={true} 
    elevation="sm"
    size="lg"
    iconData={comment}/> -->
  

</section>


<!-- Card declarations that your components
    should be able to satisfy-->
<h3>Cards</h3>
<section class="container grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-2 mx-auto p-10">
 
<!-- <Card title="Vegeta"
          subtitle="Prince of Sayans"
          description="Lorem ipsum ....."
          hasImage={true}
          imgSrc="https://qph.fs.quoracdn.net/main-qimg-40ccab97c4b182082c3525bb34575a37.webp"
          elevation="lg"
          >
        
        </Card> -->

<!-- <Card title="Svelte"
          subtitle="Javascript Framework"
          description="Lorem ipsum ....."
          hasImage={true}
          imgSrc="https://i0.wp.com/programmingwithmosh.com/wp-content/uploads/2019/12/1_OJLglSTFZ1PbwpRG0U2xXA.png?ssl=1"
          elevation="sm"
          >
        
        </Card> -->

<!-- nesting Button in Card -->

<!-- <Card title="Card with buttons"
          subtitle="No Image"
          >

      <Button fab={true} 
        elevation="lg"
        iconData={comment}/>

        </Card> -->
 
 
  <!-- <Card title="Tailwind"
          subtitle="Design"
          description="Lorem ipsum ....."
          hasImage={true}
          shaped={true}
          imgSrc="https://pbs.twimg.com/profile_images/895274026783866881/E1G1nNb0.jpg"
          elevation="lg"
          >
        
        </Card> -->


      <!-- Come up with your own bonus card attribute for this one.
      Doesnt have to fit the vuetify design pattern. Could be animation, styling, etc-->  

<!-- <Card title="Bonus"
          subtitle="Your own bonus property"
          description="Lorem ipsum ....."
          hasImage={true}
          shaped={true}
          imgSrc="https://www.travelweek.ca/wp-content/uploads/2020/04/Travel-Edge-investing-50-million-in-signing-bonus-incentive-for-luxury-travel-advisors.jpg"
          bonus={true}
          >
        
        </Card> -->

</section>
