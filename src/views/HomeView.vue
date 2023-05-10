<script setup>
import headerComponent from '../components/headerComponent.vue';
import footerComponent from '../components/footerComponent.vue';
</script>

<template>
  <div class="overview">
    <headerComponent/>
    
    <main> 
      <div class="header">
      <h1>Overview</h1>
      <div class="headerButtons">
        <button aria-label="filter">
          <img src="../assets/icons/iconFilter.png" alt="">
          <span> Filter</span>
        </button>
        <button aria-label="export">
          <img src="../assets/icons/iconExport.png" alt="">
          <span>Export</span>
        </button>
      </div>
    </div>
      <section class="graphSection">
        <div class="graphBox">
          <section  class="graphHeader">
            <h2>Today's user logins</h2>
            <div>
              <img src="../assets/icons/iconMore.png" alt="">
            </div>
          </section>
          <div class="comingSoon">
            <p>Coming Soon</p>
          </div>
          <div class="viewReport">
            <RouterLink to="/report">
              <button> View full report</button> 
            </RouterLink>
          </div>
        </div>
        <div class="graphBox">
          <section class="graphHeader">
            <h2>Average Watch time</h2>
            <div>
              <img src="../assets/icons/iconMore.png" alt="">
            </div>
          </section>
          <p>This tracks the average watch by user every month</p>
          <div class="comingSoon">
            <p>Coming Soon</p>
          </div>
        </div>
        
      </section>
      <div class="firstTable"> 
        <section class="firstTableHeading"  >
          <div> 
            <h2>Upcoming movie premieres</h2>
            <p>keep track of upcoming movie premieres</p>
          </div>
          <div class="searchBar">
            <div>
              <img src="../assets/icons/iconSearch.png" alt="">
            </div>
            <input type="text" name="search" id="" placeholder="Search" >
          </div>
        </section>
        <table>
        <tr>
          <th class="headername">
            <input type="checkbox" name="" id="">
            <span>Name</span>
            <span>
              <img src="../assets/icons/iconArrowDown.png" alt="">
            </span>
          </th>
          <th>Category</th>
          <th>Watchlists</th>
          <th>Owner</th>
          <th>Premier Date</th>
          <th></th>
        </tr>
        <tr>
          <td class="name">
            <img src="../assets/images/avengersImage.png" alt="">
            <span>Avengers Black Widow</span>
          </td>
          <td>
            <span class="genre">ACTION</span>
            <span class="genre">THRILLER</span>
          </td>
          <td>389,234</td>
          <td>Sony Entertainment</td>
          <td>21th May, 2022</td>
          <td class="view">View</td>
        </tr>
        <tr>
          <td class="name">
            <img src="../assets/images/moonlightImage.png" alt="">
            <span>Moonlight</span>
          </td>
          <td>
            <span class="genre">TRUE STORY</span>
            <span>+2 more</span>
          </td>
          <td>5,893</td>
          <td>A24 and Plan B Entertainment</td>
          <td>15th August, 2022</td>
          <td class="view">View</td>
        </tr>
        <tr>
          <td class="name">
            <img src="../assets/images/grimabyImage.png" alt="">
            <span>Grimsby</span>
          </td>
          <td>
            <span class="genre">COMEDY</span>
            <span class="genre">CRIME</span>
          </td>
          <td>200,901</td>
          <td>Sony Entertainment</td>
          <td>5th October, 2022</td>
          <td class="view">View</td>
        </tr>
        <tr>
          <td class="name">
            <img src="../assets/images/spiderman.png" alt="">
            <span>Spider Man - No way home</span>
          </td>
          <td>
            <span class="genre">ACTION</span>
            <span class="genre">THRILLER</span>
          </td>
          <td>509,262</td>
          <td>Sony Entertainment</td>
          <td>25th December, 2022</td>
          <td class="view">View</td>
        </tr>
        
      </table>
      <p class="upcoming">
        <RouterLink to="">View all upcoming premiers</RouterLink>
      </p>
      
      </div> 
     <section class="secondTable">
      <div class="secondTableHeading">
        <div >
          <h2>Trending movies</h2>
          <p>keep track of trending movie premieres</p>
        </div>
        <div class="searchBar">
            <div>
              <img src="../assets/icons/iconSearch.png" alt="">
            </div>
            <input type="text" name="search" id="" placeholder="Search" />
        </div>
      </div>
        
        <table>
        <tr>
          <th class="headername">
            <input type="checkbox" name="" id="">
            <span>Name</span>
            <span>
              <img src="../assets/icons/iconArrowDown.png" alt="">
            </span>
          </th>
          <th>Category</th>
          <th>Watchlists</th>
          <th>Owner</th>
          <th>Premier Date</th>
          <th></th>
        </tr>
       
        <tr>
          <td class="name">
            <img src="../assets/images/moonlightImage.png" alt="">
            <span>Moonlight</span>
          </td>
          <td>
            <span class="genre">TRUE STORY</span>
            <span>+2 more</span>
          </td>
          <td>5,893</td>
          <td>A24 and Plan B Entertainment</td>
          <td>15th August, 2022</td>
          <td class="view">View</td>
        </tr>
        <tr>
          <td class="name">
            <img src="../assets/images/grimabyImage.png" alt="">
            <span>Grimsby</span>
          </td>
          <td>
            <span class="genre">COMEDY</span>
            <span class="genre">CRIME</span>
          </td>
          <td>200,901</td>
          <td>Sony Entertainment</td>
          <td>5th October, 2022</td>
          <td class="view">View</td>
        </tr>
        <tr>
          <td class="name">
            <img src="../assets/images/spiderman.png" alt="">
            <span>Spider Man - No way home</span>
          </td>
          <td>
            <span class="genre">ACTION</span>
            <span class="genre">THRILLER</span>
          </td>
          <td>509,262</td>
          <td>Sony Entertainment</td>
          <td>25th December, 2022</td>
          <td class="view">View</td>
        </tr>
        </table>
        <p class="upcoming">
          <RouterLink to="">View all upcoming premiers</RouterLink>
        </p>
       
     </section>
    </main>
    <footerComponent/>
  </div>
</template>
<style scoped>
  .overview {
      color: #464951;
      display: grid;
      grid-template-columns: 1fr;
      place-items: center;
      place-content: center;
      font-family: Helvetica Neue;
      width: 85.4rem;
      margin: auto;
      line-height: 1.5;
  }
  .header {
    display: flex;
    justify-content: space-between;
    width: 82rem;
    margin: auto;
    padding: 1em 3.4em;
    color: #000000;
    
  }
  header h1 {
    font-size: 1.5rem;
  }
  .headerButtons {
    display: flex;
    gap: 2em;
  }
  .header button {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 0.5em;
    padding: 0.8em 1.2em;
    border-radius: 0.3em;
    background-color: inherit;
    border: 0.1em solid #E5E5E5;
  }
  main {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    width: 82em;
    margin: auto;
  }
  
  .graphSection {
    display: grid;
    grid-template-columns: 1fr 2fr;
    width: 82em;
    padding: 1em 4em;
    gap: 2em;
  }
  .graphBox {
    border: 0.1em solid #E5E5E5;
    height: 22em;
  }
  .graphBox p {
    color: #6A6A6A;
    font-weight: 500;
    padding: 0.5em 1.2em;
  }
  .graphHeader {
    display: flex;
    justify-content: space-between;
    align-items: center;
    color: #000000;
    font-size: 0.8rem;
    padding: 0.5em 1.2em;
  }
  .viewReport {
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    background-color: #F5F5F5;
    border: 1px solid #E0E0E0;
    width: 100%;
    height: 4.5rem;
  }
  .viewReport button {
    display: inline-block;
    padding: 0.4em 1.2em;
    background-color: #FFFFFF;
    border: 1px solid #E0E0E0;
    border-radius: 0.6em;
    color: #000000;  
    margin: 1.4em 1em;  
  }
  .comingSoon p {
    background: linear-gradient(273.64deg,#35c3f3 11.27%,#8b9fe8 36.72%,#e681d8 61.72%,#ffa9a4 82.79%,#fed2ce 107.29%,#fed2ce 107.29%);
    font-weight: 700;
    font-size: 2.5rem;
    height: 5.9em;
    -webkit-background-clip: text;
    background-clip: text;
    -webkit-text-fill-color: transparent;
  }
  .firstTable {
    display: grid;
    grid-template-columns: 1fr;
    place-content: center;
    gap: 2em;
  }
  .firstTableHeading, .secondTableHeading {
    display: flex;
    justify-content: space-between;
    width: 74em;
    margin: auto;
  }
  .searchBar input {
    outline: none;
    /* overflow-x: visible; */
 }
  
  .searchBar {
    display: flex;
    flex-direction: row;
    align-items: center;
    border: 0.1em solid #E0E0E0;
    padding: 1em;
    gap: 0.5em;
    width: 15em;
    border-radius: 0.6em;
    height: 2em;
  }
  .searchBar img {
    margin-top: 0.45em;
  }
  table {
    width: 74em;
    margin: 0 auto;    
    border-collapse: collapse;
    border-bottom: none;
  }  
  th {
    text-align: left;
  }
  tr {
    height: 4.5em;  
    border: 0.1em solid #ddd;
  }
  .secondTable {
    display: grid;
    grid-template-columns: 1fr;
    gap: 2em;
    width: 84.3em;
    padding: 1em 3em;
    margin: 0;
  }
  .upcoming {
    display: flex;
    flex-direction: row;
    margin:-2em auto auto auto;
    background-color: #F5F5F5;
    width:80em;
    height: 3.5em; 
  }
  .upcoming a {
    color: #000000;
    height: 2.2em;
    padding: 0.3em;
    width: 15em;
    text-align: center;
    margin-left: 63.6em;
    margin-top: 0.8em;
    margin: 0.8em auto auto 63.6em;
    background-color: #FFFFFF;
    border: 0.1em solid #E0E0E0;
    border-radius: 0.6em;
  }
  .view {
    display: flex;
    align-items: center;
    justify-content: center;
    border: 0.1em solid #e0e0e0;
    border-radius: 0.6em;
    cursor: pointer;
    padding: 0.6em;
    height: 2.2em;
    font-weight: 500;
    font-size: 1rem;
    margin: 1.2em;
  }
  .view:hover {
    background-color:#e0e0e0;
    color: white;
  }
  .genre  {
    padding: 0.5em 0.7em;
    width: 2em;
    margin-right: 0.5em;
    background-color: #D1D8F7;
    border-radius: 2em;
  }
  .name, .headername {
    margin-left: 0.8em;
    margin-top: 1.5em;
    /* height: 3em; */
    display: flex;
    gap: 0.5em;
    align-items: center;
    line-height: 2em;
  }
  .headername img {
    margin-top: 0.54em;
  }
</style>
