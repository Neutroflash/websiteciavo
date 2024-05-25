<script>
  import { page } from '$app/stores';
  import { Navbar, NavBrand, NavLi, NavUl, NavHamburger, ImagePlaceholder, Skeleton, TextPlaceholder } from 'flowbite-svelte';
  $: activeUrl = $page.url.pathname;
</script>

<svelte:head>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Comfortaa:wght@300..700&family=Jersey+25&family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&family=Sora:wght@100..800&display=swap" rel="stylesheet">
</svelte:head>

<div class="relative px-8 mb-0">
  <Navbar class="px-2 sm:px-4 py-2.5 fixed w-full z-20 top-0 start-0 border-b">
    <NavBrand href="/">
      <div class="h-full w-full m-0">
        <img src="https://static.wixstatic.com/media/c5cdf7_60ce9302148b452f813f0d4ec0714528~mv2.png/v1/fill/w_37,h_57,al_c,q_95,enc_auto/logociavolella_edited.png" class="me-3 h-full " alt="Flowbite Logo" />
      </div>
      <div class="flex flex-col justify-center items-center h-full">
        <span class="self-start whitespace-nowrap text-[40px] font-bold text-[#555555] tracking-normal leading-[1.1em] text-center">CIAVOLELLA</span>
        <span class="self-center whitespace-nowrap text-[15px] font-semibold text-[#CC0207] tracking-[.21em] leading-[1.1em]">Engineering Consulting</span>
      </div>
    </NavBrand>
    <NavHamburger/>
    <NavUl {activeUrl}>
      <NavLi href="/" active={false}>HOME</NavLi>
      <NavLi href="#services">SERVICES</NavLi>
      <NavLi href="#company">COMPANY</NavLi>
      <NavLi href="#contacts">CONTACTS</NavLi>
      <NavLi href="">PROJECTS</NavLi>
      <NavLi href="">CAREER</NavLi>
    </NavUl>
  </Navbar>
</div>

