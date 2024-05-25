<script>
  import { Footer, FooterCopyright, FooterLinkGroup, FooterLink, FooterBrand, FooterIcon } from 'flowbite-svelte';
  import { FacebookSolid, GithubSolid, DiscordSolid, TwitterSolid, GoogleSolid, LinkedinSolid} from 'flowbite-svelte-icons';
</script>

<Footer footerType="socialmedia" class="!bg-[#F5F5F5]">
  <div class="md:flex md:justify-evenly">
    <div class="mb-6 md:mb-0 flex justify-center items-center">
      <FooterBrand imgClass="" href="/" src="https://static.wixstatic.com/media/c5cdf7_60ce9302148b452f813f0d4ec0714528~mv2.png/v1/fill/w_37,h_57,al_c,q_95,enc_auto/logociavolella_edited.png" alt="Ciavolella Logo"/>
      <div class="flex flex-col justify-end ml-4">
        <h1 class="self-start whitespace-nowrap text-[40px] font-bold text-[#555555] tracking-normal leading-[1.1em] text-center">CIAVOLELLA</h1>
        <span class="self-center whitespace-nowrap text-[15px] font-semibold text-[#CC0207] tracking-[.21em] leading-[1.1em]">Engineering Consulting</span>
      </div>
    </div>
    <div class="grid grid-flow-col w-[70%] justify-around">
      <div class="mr-[2rem]">
        <h2 class="mb-6 text-sm font-semibold text-gray-900 uppercase dark:text-white">Ciavolella S.r.l.</h2>
        <FooterLinkGroup>
          <FooterLink liClass="mb-4" href="/">Via Di Biasio, 144<br>03043 - Cassino (Fr), Italy</FooterLink>
          <FooterLink liClass="mb-4" href="/">+39 0776 311097</FooterLink>
          <FooterLink liClass="mb-4" href="/">info@ciavolella.com </FooterLink>
          <FooterLink liClass="mb-4" href="/">P.IVA 02831730607</FooterLink>
        </FooterLinkGroup>
      </div>
      <div class="ml-[2rem] mr-[2rem]">
        <h2 class="mb-6 text-sm font-semibold uppercase text-gray-900 dark:text-white">Naviga</h2>
        <FooterLinkGroup>
          <FooterLink liClass="mb-4" href="/">Services</FooterLink>
          <FooterLink liClass="mb-4" href="/">Company</FooterLink>
          <FooterLink liClass="mb-4" href="/">Contacts</FooterLink>
          <FooterLink liClass="mb-4" href="/">Projects</FooterLink>
          <FooterLink liClass="mb-4" href="/">Career</FooterLink>
        </FooterLinkGroup>
      </div>
      <div class="ml-[2rem] mr-[2rem]">
        <h2 class="mb-6 text-sm font-semibold uppercase text-gray-900 dark:text-white">Social networks</h2>
        <FooterLinkGroup>
          <FooterLink liClass="mb-4" href="/">Google Plus</FooterLink>
          <FooterLink liClass="mb-4" href="/">Linkedin</FooterLink>
        </FooterLinkGroup>
      </div>
      <div class="w-[20rem] ml-[2rem] mr-[2rem]">
        <h2 class="mb-6 text-sm font-semibold uppercase text-gray-900 dark:text-white">Lavora con noi</h2>
        <FooterLinkGroup>
          <FooterLink liClass="mb-4" href="/">Ciavolella engineering è  alla ricerca di persone appassionate, dinamiche, aperte  alla collaborazione e al confronto con voglia di cimentarsi in un ambiente nuovo e in crescita.</FooterLink>
          <FooterLink liClass="mb-4" href="/">Clicca qui e scopri le posizioni aperte.</FooterLink>
        </FooterLinkGroup>
      </div>
    </div>
  </div>
  <hr class="my-6 border-[black] sm:mx-auto dark:border-gray-700 lg:my-8" />
  <div class="sm:flex sm:items-center sm:justify-between">
    <FooterCopyright href="/" by="- Ciavolella srl -" />
    <div class="flex mt-4 space-x-6 rtl:space-x-reverse sm:justify-center sm:mt-0">
      <FooterIcon href="/">
        <LinkedinSolid class="w-5 h-5 text-gray-500 dark:text-gray-500 hover:text-gray-900 dark:hover:text-white" />
      </FooterIcon>
      <FooterIcon href="/">
        <GoogleSolid class="w-5 h-5 text-gray-500 dark:text-gray-500 hover:text-gray-900 dark:hover:text-white" />
      </FooterIcon>
    </div>
  </div>
</Footer>

  <style>
    
  </style>