<template> 
  
  <v-app id="inspire">
    <v-navigation-drawer
      floating
      permanent
      v-model="drawer"
      app
      class="pt-4"
      color="grey lighten-3"
      mini-variant 
    >
     
      <div class="mx-3 py-3"> 
       
        <v-btn
          icon small class="p-5"
          to="/"   >
          <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
            <path stroke-linecap="round" stroke-linejoin="round" d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6" />
          </svg>
        </v-btn> 
      </div>


      <div class="mx-3 py-1.5 "> 
        <v-btn
          icon small class="p-5"
          to="/"   >
            <!-- <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
              <path stroke-linecap="round" stroke-linejoin="round" d="M3 5h12M9 3v2m1.048 9.5A18.022 18.022 0 016.412 9m6.088 9h7M11 21l5-10 5 10M12.751 5C11.783 10.77 8.07 15.61 3 18.129" />
            </svg> -->
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
              <path stroke-linecap="round" stroke-linejoin="round" d="M21 13.255A23.931 23.931 0 0112 15c-3.183 0-6.22-.62-9-1.745M16 6V4a2 2 0 00-2-2h-4a2 2 0 00-2 2v2m4 6h.01M5 20h14a2 2 0 002-2V8a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
            </svg>
        </v-btn> 
        <span class="text-xs font-light px-1"> 介紹 </span>
      </div>

      <div class="mx-3 pt-3 py-1.5 "> 
        <v-btn
          icon small class="p-5"
          to="/introList_CASE1"   >
              <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                <path stroke-linecap="round" stroke-linejoin="round" d="M9.663 17h4.673M12 3v1m6.364 1.636l-.707.707M21 12h-1M4 12H3m3.343-5.657l-.707-.707m2.828 9.9a5 5 0 117.072 0l-.548.547A3.374 3.374 0 0014 18.469V19a2 2 0 11-4 0v-.531c0-.895-.356-1.754-.988-2.386l-.548-.547z" />
              </svg>
        </v-btn> 
        <span class="text-xs font-light px-1"> 理念 </span>
      </div>

      <div class="mx-3 py-1.5 "> 
        <v-btn
          icon small class="p-5"
          to="/studyList_CASE1"   >
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
              <path stroke-linecap="round" stroke-linejoin="round" d="M12 6.253v13m0-13C10.832 5.477 9.246 5 7.5 5S4.168 5.477 3 6.253v13C4.168 18.477 5.754 18 7.5 18s3.332.477 4.5 1.253m0-13C13.168 5.477 14.754 5 16.5 5c1.747 0 3.332.477 4.5 1.253v13C19.832 18.477 18.247 18 16.5 18c-1.746 0-3.332.477-4.5 1.253" />
            </svg> 
        </v-btn> 
        <span class="text-xs font-light px-1"> 文獻 </span>
      </div>  

      <!-- <div class="mx-3 py-1.5 "> 
        <v-btn
          icon small class="p-5"
          to="/greatList_CASE1"   >
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
              <path stroke-linecap="round" stroke-linejoin="round" d="M11.049 2.927c.3-.921 1.603-.921 1.902 0l1.519 4.674a1 1 0 00.95.69h4.915c.969 0 1.371 1.24.588 1.81l-3.976 2.888a1 1 0 00-.363 1.118l1.518 4.674c.3.922-.755 1.688-1.538 1.118l-3.976-2.888a1 1 0 00-1.176 0l-3.976 2.888c-.783.57-1.838-.197-1.538-1.118l1.518-4.674a1 1 0 00-.363-1.118l-3.976-2.888c-.784-.57-.38-1.81.588-1.81h4.914a1 1 0 00.951-.69l1.519-4.674z" />
            </svg>
        </v-btn> 
        <span class="text-xs font-light "> 成果 </span>
      </div> 

      <div class="mx-3 py-1.5.5 "> 
        <v-btn
          icon small class="p-5"
          to="/shareList_CASE1"   >
              <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                <path stroke-linecap="round" stroke-linejoin="round" d="M12 10v6m0 0l-3-3m3 3l3-3m2 8H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z" />
              </svg> 
        </v-btn> 
        <span class="text-xs font-light "> 分享 </span>
      </div> -->

      <v-divider class="pt-2"></v-divider> 

      <div class="mx-3 py-1.5 "> 
        <v-btn
          icon small class="p-5"
          to="/emailme"   >
          <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
            <path stroke-linecap="round" stroke-linejoin="round" d="M7 8h10M7 12h4m1 8l-4-4H5a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v8a2 2 0 01-2 2h-3l-4 4z" />
          </svg>
        </v-btn> 
      </div>

      <div class="mx-3 py-1.5 "> 
        <v-btn
          icon small class="p-5"
          to="Login_ing"   >
          <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
            <path stroke-linecap="round" stroke-linejoin="round" d="M12 6V4m0 2a2 2 0 100 4m0-4a2 2 0 110 4m-6 8a2 2 0 100-4m0 4a2 2 0 110-4m0 4v2m0-6V4m6 6v10m6-2a2 2 0 100-4m0 4a2 2 0 110-4m0 4v2m0-6V4" />
          </svg>
        </v-btn> 
      </div> 

<!-- @click="getAnysisReport" -->
      <!-- <div class="mx-3 py-1.5 "> 
        <v-btn
          icon small class="p-5"
          to="Blog_v1"
           >
          <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
            <path stroke-linecap="round" stroke-linejoin="round" d="M15.232 5.232l3.536 3.536m-2.036-5.036a2.5 2.5 0 113.536 3.536L6.5 21.036H3v-3.572L16.732 3.732z" />
          </svg>
        </v-btn> 
      </div>  -->
      

    <v-divider class="pt-2"></v-divider>

      <div class="mx-2 py-1.5 "> 
        <v-btn
          small fab class="p-5 bg-gray-100 text-gray-600 "
          to="1"   >首頁1 
        </v-btn> 
      </div> 

      <div class="mx-2 py-1.5 "> 
        <v-btn
          small fab class="p-5 bg-gray-100 text-gray-600 "
          to="2"   >首頁2 
        </v-btn>
      </div> 

      <div class="mx-2 py-1.5 "> 
        <v-btn
          small fab class="p-5 bg-gray-100 text-gray-600 "
          to="3"   >首頁3 
        </v-btn>
      </div> 

       <!-- text icon class="ma-2" 
        color="black" 
        to="Login_ing" -->

    </v-navigation-drawer>
 

    
    <v-main>  
     <router-view />
    </v-main> 
  </v-app>

  
</template>

<script>
export default {
    data: () => ({
      direction: 'top',
      fab: false,
      fling: false,
      hover: false,
      tabs: null,
      top: false,
      right: true,
      bottom: true,
      left: false,
      transition: 'slide-y-reverse-transition',
    }),
    methods: {
      getAnysisReport(){
    

              Swal.fire({
              icon: 'question',
              title: '是否好奇 測試完的結果?',
              text: '讓我 分析數據後,帶您了解 相關的診斷 建議',
              footer: '<a href=""> 重新測驗 </a>'
            })
          },
    },

    watch: {
      top (val) {
        this.bottom = !val
      },
      right (val) {
        this.left = !val
      },
      bottom (val) {
        this.top = !val
      },
      left (val) {
        this.right = !val
      },
    },
  }
</script>