<script setup lang="ts">
import Logo from "@/assets/svg/logo.svg";
import Facebook from "@/assets/svg/facebook.svg";
import Tiktok from "@/assets/svg/tiktok.svg";
import LinkedIn from "@/assets/svg/linkedin.svg";
import Snapchat from "@/assets/svg/snapchat.svg";
import Youtube from "@/assets/svg/youtube.svg";
</script>

<template>
   <footer class="App-Footer">
      <div class="Logo-Groupe Tanou International™">
         <img :src="Logo" alt="Groupe Tanou International™" />
         <p>
            Groupe Tanou International™ is an innovative Burkinabè company specialized
            in international trade, export and product sourcing, logistics, and business travel.
            Founded by experts in sino-african relations and commercial operations, 
            the group is committed to facilitating exchanges and commercial operations,
            between Africa, Asia and the world relations.
         </p>
      </div>
      <div class="Icon-Row Outer-Icon-Row-externe">
         <a href="https://www.facebook.com/share/15mrzcJWYF/?mibextid=wwXIfr" target="_blank"> 
            <img :src="Facebook" alt="facebook" />
         </a>  
         <a href="https://www.tiktok.com/@groupe.tanou.inte?_t=ZM-8wCYY70bP1T&_r=1" target="_blank">     
            <img :src="Tiktok" alt="tiktok" />
         </a>         
         <a href="https://www.linkedin.com/company/groupe-tanou-international%E2%84%A2/" target="_blank">         
                  <img :src="LinkedIn" alt="linkedin" />
         </a>      
         <a href="https://www.snapchat.com/add/groupetanou?share_id=NNHvNhInQGA&locale=fr-FR" target="_blank">  
               <img :src="Snapchat" alt="snapchat" />
         </a>            
         <a href="https://youtube.com/@groupetanou?si=8uxi7qpQrOusLaPu" target="_blank">     
                  <img :src="Youtube" alt="youtube" />
         </a>    
      </div>
      <nav class="Links-Container">
         <li class="Links">
            <h3>INFO</h3>
            <ul>
               <li>About Cadence</li>
               <li>Help & Support</li>
               <li>FAQs</li>
               <li>Return Policy</li>
               <li>Terms of Use</li>
            </ul>
         </li>
         <li class="Links">
            <h3>SERVICES</h3>
            <ul>
               <li>Transportation</li>
               <li>Delayed Deliveries</li>
               <li>Packaging</li>
            </ul>
         </li>
         <li class="Links">
            <h3>COMPANY</h3>
            <ul>
               <li>Privacy Policy</li>
               <li>Careers</li>
               <li>Management</li>
            </ul>
         </li>
         <li class="Links Contact-Links">
            <h3>CONTACT</h3>
            <div class="Icon-Row">
               <img :src="Facebook" alt="facebook icon" />
               <img :src="Tiktok" alt="tiktok icon" />
               <img :src="LinkedIn" alt="linkedin icon" />
               <img :src="Snapchat" alt="snapchat icon" />
               <img :src="Youtube" alt="youtube icon" />
            </div>
         </li>
      </nav>
      <p class="Copyright">Copyright © 2025 - GROUPE TANOU INTERNATIONAL™. All rights reserved.</p>
   </footer>
</template>

<style scoped>
.App-Footer {
   position: relative;
   display: grid;
   grid-template-columns: 25% 65%;
   column-gap: 10%;
   place-items: center;
   height: 430px;
   background: #11567d29;
   padding-inline: var(--Vertical-Squeeze);
}
.Logo-Container img {
   height: 66px;
}
.Logo-Container p {
   max-width: 400px;
   font-weight: 700;
   font-size: 13px;
   line-height: 16px;
   color: #125e8a;
}

.Links-Container {
   display: grid;
   grid-template-columns: repeat(4, 25%);
   width: 100%;
}
.Links h3 {
   font-family: "Raleway";
   font-weight: 700;
   font-size: 28px;
   background: linear-gradient(94.74deg, #3c92ca 10.56%, #125e8a 94.88%);
   -webkit-background-clip: text;
   -webkit-text-fill-color: transparent;
   background-clip: text;
   margin-bottom: 10px;
}
.Links li {
   font-weight: 400;
   font-size: 16px;
   line-height: 19px;
   margin-bottom: 8px;
   color: #125e8a;
}
.Icon-Row {
   display: grid;
   grid-template-columns: auto auto auto auto;
   column-gap: 5px;
   width: fit-content;
}
.Outer-Icon-Row {
   display: none;
}

.Copyright {
   position: absolute;
   bottom: 0;
   font-family: "Product Sans";
   font-style: normal;
   font-weight: 400;
   font-size: 19.0317px;
   line-height: 23px;
   text-align: center;
   margin-bottom: 40px;
   color: #11567d;
}
@media (max-width: 1024px) {
   .Logo-Container img {
      height: 50px;
   }
   .Links h3 {
      font-size: 20px;
   }
   .Links li {
      font-size: 14px;
   }
}
@media (max-width: 768px) {
   .App-Footer {
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      height: 540px;
   }
   .Logo-Container {
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
   }
   .Logo-Container img {
      height: 60px;
   }
   .Logo-Container p {
      text-align: center;
      width: 95%;
      font-size: 11pt;
      line-height: 19px;
      margin-bottom: 0;
   }
   .Outer-Icon-Row {
      display: grid;
      column-gap: 13px;
      margin-block: 40px;
   }
   .Icon-Row img {
      height: 35px;
   }
   .Links-Container {
      display: flex;
      justify-content: space-around;
      padding-inline: var(--Vertical-Squeeze);
      margin-bottom: 30px;
   }
   .Links {
      display: flex;
      align-items: center;
      flex-direction: column;
   }
   .Links > * {
      text-align: center;
   }
   .Links li {
      font-size: 13pt;
   }
   .Links.Contact-Links {
      display: none;
   }
}
@media (max-width: 425px) {
   .Logo-Container p {
      font-size: 9pt;
   }
   .Links h3 {
      font-size: 15px;
   }
   .Links li {
      font-size: 10pt;
   }
   .Copyright {
      font-size: 10pt;
   }
}
</style>
