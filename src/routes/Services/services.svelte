
<!-- Import images from assets folder  -->
<script>
    import Building from "../../assets/BIM.png"
    import Design from "../../assets/design.png"
    import Admin from "../../assets/admin.png"
    import Counter from './Counter.svelte'
    import Carousel from 'svelte-carousel'
    import { browser } from '$app/environment';
    import { Button } from 'flowbite-svelte';
    import { ThumbsUpSolid, ArrowRightOutline, ArrowLeftOutline } from 'flowbite-svelte-icons';

    let carousel;
    const handleNextClick = () => {
    carousel.goToNext()
  }
  const handlePrevClick = () => {
    carousel.goToPrev()
  }

</script>

<div class="conteiner-carousel-divs">
    {#if browser}
<Carousel
  bind:this={carousel}
  autoplay
  autoplayDuration={8000}
  autoplayProgressVisible
  pauseOnFocus
>

<div slot="next" class="flex w-full h-full justify-end items-center m-0 bg-transparent absolute">
    <Button on:click={handleNextClick} pill class="!p-2 m-3 bg-sky-400 hover:bg-[#8B0000]"><ArrowRightOutline class="w-6 h-6" /></Button>
</div>

<div slot="prev" class="flex w-1/2 h-full justify-start items-center m-0 bg-transparent absolute z-[1]">
    <Button on:click={handlePrevClick} pill class="!p-2 m-3  bg-sky-400 hover:bg-[#8B0000]"><ArrowLeftOutline class="w-6 h-6" /></Button>
</div>

  <div class="continer-div-1">
        <h5 class="mb-2 font-bold tracking-tight text-gray-50  text-6xl !bg-pink-500 pl-4"><b>BIM</b></h5>
        <p class="font-bold tracking-tight text-white text-2xl mt-8 mb-8"><b>FOR</b></p>
        <p class="mb-6 font-bold tracking-tight text-gray-50 text-4xl !bg-blue-600/80 p-4 pl-2 pr-2"><b>PHARMACEUTICAL</b></p>
        <p class="mb-2 font-bold tracking-tight text-gray-50 text-4xl !bg-sky-500/80"><b>PLANTS</b></p>
    
  </div>
  <div class="continer-div-2">
    
        <h5 class="mb-2 font-bold tracking-tight text-gray-50  text-6xl !bg-pink-500 pl-4"><b>BIM</b></h5>
        <p class="font-bold tracking-tight text-gray-600 text-2xl mt-8 mb-8"><b>FOR</b></p>
        <p class="mb-6 font-bold tracking-tight text-gray-50 text-4xl !bg-blue-600/80 p-4 pl-2 pr-2"><b>PHARMACEUTICAL</b></p>
        <p class="mb-2 font-bold tracking-tight text-gray-50 text-4xl !bg-sky-500/80"><b>PLANTS</b></p>
    
  </div>
  <div class="continer-div-3">
    <div class="!bg-sky-400/50 w-full h-full flex justify-center items-center flex-col">
        <h1 class="mb-2 font-bold tracking-tight text-gray-50  text-9xl">BIM</h1>
        <p class="text-[#8B0000] mb-2 font-semibold text-2xl " style="letter-spacing: 0.25em; word-spacing: 0.25em;">the new design methodology</p>
        <Button class="mt-[8rem] bg-[#8B0000] hover:bg-white hover:text-[#8B0000] " size="md" pill href="#">MORE ABOUT US</Button>
    </div>
  </div>
  <div class="continer-div-4">
    <div class="flex justify-start align-middle flex-col">
    <p class="text-[#8B0000] mb-2 text-4xl mt-12 font-mono" style="letter-spacing: 0.10em">Detail Engineering</p>
    <p class="text-[#8B0000] mb-2 text-4xl font-mono" style="letter-spacing: 0.10em">We love complex projects...</p>
    <Button class="mt-[5rem] bg-[#8B0000] hover:bg-white hover:text-[#8B0000] w-48" pill href="#">MORE ABOUT US</Button>
    </div>
  </div>
  <div class="continer-div-5">
    <div class="!bg-sky-600/60 w-full h-full flex justify-center items-center flex-col">
        <p class="text-[white] mb-2 font-bold text-5xl font-mono">Efficient detailing</p>
        <p class="text-[#BADA55] mb-2 font-bold text-5xl font-mono mt-12">makes</p>
        <p class="text-[white] mb-2 font-bold text-5xl font-mono mt-12">a big complex steelwork</p>
        <p class="text-[white] mb-2 font-bold text-5xl font-mono mt-12">simple, fast and easy</p>
    </div>
  </div>
  <div class="continer-div-6"></div>
</Carousel>
{/if}
</div>

<!-- SERVICES MAIN PAGE -->

<div class="section-services">
    <h1 class="title-services">SERVICES</h1>
    <hr class="separator">
    <p class="text-title">Our multidisciplinary engineering services</p>
</div>
<div class="text-services">
    <div class="text1">
        Ciavolella engineering provides highly qualified services in <span style="color: #555555"><b>Design & Engineering
            Project Management, Construction Management</b></span> and we make them even better througth <span style="color: #555555; text-decoration: underline"><b>BIM</b></span> (Building information modeling) methodology.
    </div>
    <div class="text2">
        "Commited to innovattion and excellent in all we do"
    </div>
    <div class="text3">
        Our main Sectors:
        <ol type="A">
            <li style="pointer-events: none; cursor: default;">Pharmaceutical</li>
            <li style="pointer-events: none; cursor: default;">Life sciencie, and healthcare</li>
            <li style="pointer-events: none; cursor: default;">Chemical</li>
            <li style="pointer-events: none; cursor: default;">Industrial</li>
        </ol>
    </div>
</div>
<div class="cards-services">
    <div class="cards">
        <a href="#">
            <div class="conteiner-img">
                <img src={Design} alt="Designimg">
            </div>
        </a>
        <a href="#" style="color: black;">
            <p class="text-cards"><b>Design</b></p>
        </a>
        <ul>
            <li class="lista-cards" style="pointer-events: none; cursor: default;">Piping & Layout​​​​​</li>
            <li class="lista-cards">HVAC</li>
            <li class="lista-cards" style="pointer-events: none; cursor: default;">Clean Room ​</li>
            <li class="lista-cards" style="pointer-events: none; cursor: default;">Stress Analysis & Support​</li>
            <li class="lista-cards" style="pointer-events: none; cursor: default;">Process</li>
            <li class="lista-cards" style="pointer-events: none; cursor: default;">Civil & Structures</li>
            <li class="lista-cards" style="pointer-events: none; cursor: default;">Architectural and Building design</li>
            <li class="lista-cards">Steel detailing</li>
        </ul>
    </div>
    <div class="cards">
        <a href="#">
            <div class="conteiner-img">
                <img src={Building} alt="BIMimg">
            </div>
        </a>
            <a href="#" style="color: black;">
                <p class="text-cards"><b>BIM</b></p>
            </a>
            <ul>
                <li class="lista-cards-1">Conceptual & Detailed Design</li>
                <li class="lista-cards-1">Analysis & Quantity Surveyors</li>
                <li class="lista-cards-1" style="pointer-events: none; cursor: default;">3D laser scanning  for an accurate <br> and complete site survey </li>
                <li class="lista-cards-1"><b>Clash Detection</b></li>
                <li class="lista-cards-1"><b>Project Managers:</b> 4D Construction<br>sequencing - 5D Cost Management & Planning Reporting</li>
                <li class="lista-cards-1">Facility management</li>
            </ul>
    </div>
    <div class="cards">
        <a href="#">
            <div class="conteiner-img">
                <img src={Admin} alt="Adminimg">
            </div>
        </a>
        <a href="#" style="color: black;">
            <p class="text-cards"><b>Management and Consultancy</b></p>
        </a>
        <ul>
            <li class="lista-cards-2" style="pointer-events: none; cursor: default;">Project Management</li>
            <li class="lista-cards-2" style="pointer-events: none; cursor: default;">Construction Management</li>
            <li class="lista-cards-2" style="pointer-events: none; cursor: default;">Project Controls</li>
            <li class="lista-cards-2" style="pointer-events: none; cursor: default;">REACH Consultancy Services</li>
            <li class="lista-cards-2" style="pointer-events: none; cursor: default;">Commissioning</li>
        </ul>
    </div>
</div>

<div class="message">
    <h1 class="text-message">WE CAN SUPPORT YOU THROUGH ALL PROJECT PHASES</h1>
   </div> 

   <!-- company section -->

<div class="company-background">
    <div class="conteiner-tilte-text">
        <div class="conteiner-company">
            <div class="conteiner-title-company">
                <h1 class="companytitle">COMPANY</h1>
                <hr class="separator-company">
                <span class="text-title-company">
                    Ciavolella engineering, a dynamic and flexible team with the aim to deliver the highest possible engineering quality to meet the client requirements.
                </span>
            </div>
            <div class="conteiner-text-company">
                <p class="text">We care very much for our customer needs. Health and Safety, quality, correct timing, and budget limits are primary goals for us.</p>
                <p class="text">The staff in Ciavolella engineering is a combinations of senior experienced engineers and young dynamic ones to form a passionate, motivated, and collaborative team.</p>
                <p class="text">We are able to provide engineering services from the first concept idea, throughout the project and the construction to the very last “as built” drawing, Comprising multidisciplinary aspects that your project may need to make it reality, well integrated in the right BIM model.</p>
            </div>
        </div>
        <div class="footer-company">
            <div class="information-ciavolella">
                <div class="Counter-years">
                    <Counter target={1980} duration={1500} />
                    <p class="text-counter">Year Estabilished</p>
                </div>
                <div class="Counter-years">
                    <Counter target={1576} duration={1500} />
                    <p class="text-counter">Projects Completed</p>
                </div>
                <div class="Counter-years">
                    <div class="align">
                        <Counter target={100} duration={1500} /><span style="font-size: 3rem;">+</span>
                    </div>
                    <p class="text-counter">Clients</p>
                </div>
                <div class="Counter-years">
                    <Counter target={7} duration={1500} />
                    <p class="text-counter">Nations</p>
                </div>
            </div>
        </div>
    </div>
</div>

<!-- Styles section -->

<style>

    @import url('https://fonts.googleapis.com/css2?family=Comfortaa:wght@300..700&family=Jersey+25&family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&family=Sora:wght@100..800&display=swap');

    .conteiner-carousel-divs{
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        width: 100%;
        margin: 0 auto;
        gap: 0;
    }

    .continer-div-1{
        margin: 0 auto;
        display: flex;
        flex-direction: column;
        align-items: end;
        justify-content: center;
        padding-right: 7%;
        width: 100%;
        height: 80vh; 
        background-image: url("https://static.wixstatic.com/media/c5cdf7_d2feb66b1bdc4bdbb93750f9112e5aa4~mv2.jpg/v1/fill/w_980,h_783,al_c,q_90,enc_auto/c5cdf7_d2feb66b1bdc4bdbb93750f9112e5aa4~mv2.jpg");
        background-size: 100% 100%;
        background-repeat: no-repeat;
    }
    .continer-div-2{
        display: flex;
        flex-direction: column;
        align-items: end;
        justify-content: center;
        padding-right: 7%;
        width: 100%;
        height: 80vh; 
        background-image: url("https://static.wixstatic.com/media/c5cdf7_e35fb71df8734505a712df4fdf9a6759~mv2.jpg/v1/fill/w_1435,h_783,al_t,q_90,enc_auto/c5cdf7_e35fb71df8734505a712df4fdf9a6759~mv2.jpg");
        background-size: 100% 100%;
        background-repeat: no-repeat;
    }

    .continer-div-3{
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
        width: 100%;
        height: 80vh; 
        background-image: url("https://static.wixstatic.com/media/c5cdf7_d2feb66b1bdc4bdbb93750f9112e5aa4~mv2.jpg/v1/fill/w_980,h_783,al_c,q_90,enc_auto/c5cdf7_d2feb66b1bdc4bdbb93750f9112e5aa4~mv2.jpg");
        background-size: 100% 100%;
        background-repeat: no-repeat;
    }

    .continer-div-4{
        display: flex;
        flex-direction: column;
        align-items: center;
        width: 100%;
        height: 80vh; 
        background-image: url("https://static.wixstatic.com/media/c5cdf7_245b8a3d426a4b22adea049082b4a631~mv2.jpg/v1/fill/w_1613,h_783,al_c,q_90,enc_auto/c5cdf7_245b8a3d426a4b22adea049082b4a631~mv2.jpg");
        background-size: 100% 100%;
        background-repeat: no-repeat;
    }

    .continer-div-5{
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
        width: 100%;
        height: 80vh; 
        background-image: url("https://static.wixstatic.com/media/c5cdf7_52390ab31b9a4b1685a5b3c32ade754b~mv2_d_3835_2078_s_2.jpg/v1/fill/w_1607,h_783,al_c,q_90,enc_auto/c5cdf7_52390ab31b9a4b1685a5b3c32ade754b~mv2_d_3835_2078_s_2.jpg");
        background-size: 100% 100%;
        background-repeat: no-repeat;
    }

    .continer-div-6{
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
        width: 100%;
        height: 80vh; 
        background-image: url("https://static.wixstatic.com/media/c5cdf7_0569da5a8a074fb591fefef9d3ef0dde~mv2.jpg/v1/fill/w_1607,h_783,al_c,q_90,enc_auto/c5cdf7_0569da5a8a074fb591fefef9d3ef0dde~mv2.jpg");
        background-size: 100% 100%;
        background-repeat: no-repeat;
    }

    /* Styles Services */

    .section-services{
        margin-top: 8rem;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        
    }

    .title-services{
        color: #AAAAAA;
        font-size: 3rem;
        font-family: "Sora", sans-serif;
    }

    .separator{
        width: 5%;
        border: 5px solid #1B99E8;
        margin: 1rem;
    }

    .text-title{
        font-size: 1.5rem;
        padding-bottom: 3rem;
        font-family: "Sora", sans-serif;
    }

    .text-services{
        background-color: #54B3EE;
        width: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
    }

    .text1{
        font-family: "Sora", sans-serif;
        color: #FFFFFF;
        margin: 25%;
        margin-top: 0;
        margin-bottom: 0;
        padding-top: 5rem;
        justify-content: center;
        font-size: 1.5rem;
    }

    .text2{
        font-family: "Sora", sans-serif;
        color: #FFFFFF;
        margin: 25%;
        margin-top: 0;
        margin-bottom: 0;
        justify-content: center;
        font-size: 1.5rem;
        padding-top: 2rem;
        padding-bottom: 2rem;
        font-style: italic;
    }

    .text3{
        font-family: "Sora", sans-serif;
        margin: 0;
        color: #FFFFFF;
        font-size: 1.5rem;
        padding-bottom: 5rem;
        margin: 25%;
        margin-top: 0;
        margin-bottom: 0;
    }

    .cards-services{
        margin-left: 0;
        margin-right: 0;
        width: 100%;
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        background-color: #F5F5F5;
    }

    .cards{
        margin: 4rem;
        border-radius: 1rem;
        display: flex;
        flex-direction: column;
        align-items: center;
        height: 600px;
        width: 350px;
    }

    .conteiner-img{
        margin: 1rem;
        margin-top: 2rem;
        border: 1px solid rgb(65, 128, 181);
        height: 160px;
        width: 160px;
        border-radius: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
        transition: 1s;
    }

    .conteiner-img:hover{
        background-color: rgba(16, 109, 176, .21);
    }

    .text-cards{
        font-family: "Sora", sans-serif;
        margin: 1rem;
        margin-top: 0;
        transition: 0.1s;
    }

    .text-cards:hover{
        color: rgb(65, 128, 181);
    }

    ul{
        list-style-type: disc;
        margin-bottom: 1rem;
    }

    li:hover{
        color: rgb(65, 128, 181);
        text-decoration: underline;
    }

    .lista-cards{
        font-family: "Sora", sans-serif;
        margin: 1rem;
        padding-top: 0;
    }

    .lista-cards-1{
        font-family: "Sora", sans-serif;
        margin: 1rem;
        padding-top: 0;
        font-size: 15px;
    }

    .lista-cards-2{
        font-family: "Sora", sans-serif;
        margin: 1rem;
        padding-top: 0;
    }

    img{
        margin: 1rem auto;
        width: 100px;
        height: 100px;
    }

    .message{
        display: flex;
        align-items: center;
        justify-content: center;
        background: linear-gradient(0deg, #54B3EE, 30% , #F5F5F5);
        margin: 0;
    }

    .text-message{
        margin: 2rem;
        font-family: "Sora", sans-serif;
        font-style: italic;
    }

    /* Company styles section*/

    .company-background{
        background-image: url(https://static.wixstatic.com/media/f7133f9895b24525a2ad16c1e778c9fa.jpg/v1/fill/w_1072,h_750,al_c,q_90,enc_auto/f7133f9895b24525a2ad16c1e778c9fa.jpg);
        background-position: center center;
        background-repeat: no-repeat;
        background-size: cover;
    }

    .conteiner-tilte-text{
        width: 100%;
        padding: 1.5rem;
        padding-bottom: 0;
        padding-left: 0;
        display: flex;
        flex-direction: column;
        align-items: start;
    }

    .conteiner-company{
        margin: 2rem;
        margin-left: 10%;
        padding: 4rem;
        width: 500px;
        justify-content: left;
        background-color: rgba(255, 255, 255, 0.9);
    }

    .conteiner-title-company{
        width: 100%;
    }

    .companytitle{
        font-family: "Sora", sans-serif;
        color: #AAAAAA;
        font-size: 3rem;
    }

    .separator-company{
        width: 30%;
        border: 5px solid #1B99E8;
        margin: 0.5rem;
        margin-left: 0;
        margin-bottom: 3rem;
    }

    .text-title-company{
        font-family: "Sora", sans-serif;
        color: #555555;
        font-size: 1.5rem;
    }

    .conteiner-text-company{
        margin: 0;
        margin-top: 2rem;
        width: 100%;
    }

    .text{
        font-family: "Sora", sans-serif;
        margin: 0 auto;
        margin-top: 1.5rem;
        margin-bottom: 1.5rem;
        color: #555555;
    }

    /* foot section of the company section */

    .footer-company{
        width: 100%;
        margin: 0;
        background-color: #1B99E8;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
    }

    .information-ciavolella{
        width: 100%;
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
        gap: 7rem;
    }

    .Counter-years{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        font-family: "Sora", sans-serif;
        margin: 2rem;
        font-size: 1.5rem;
        color: white;
    }

    .align{
        display: flex;
        align-items: center;
        justify-content: center;
    }
    
</style>