<template>
  <div class="omega_parent">
    <header class="page_header">
      <span>

        <h1>LOGO</h1>


        <h2>MENU</h2>

      </span>



    </header>
    <main class="page_main">
      <section>
        <article>
          <span class="user_profile">

            <small-user-profile v-for="(user, i) in users" :key="i" :user="users[i]" @user_click="show_user_id">
            
            
            
            
            
            </small-user-profile>

          </span>

          <span>

            <h1>{{ username }}</h1>

          </span>
        </article>
      </section>
    </main>
    <footer class="page_footer">

      <span>

        <h1>Footer text</h1>

        <h1>Footer text</h1>

      </span>


    </footer>
  </div>
</template>

<script>

import SmallUserProfile from './components/SmallUserProfile.vue';

export default {

  methods:{

    show_user_id(id){


      this.username = id;


      console.log(`I work`);

    }

  },


  data() {
    return {

      username:{



      },


      users: [{



        name: `Cameron`,

        age: `25`,

        is_premium: true,

        id: 327623

      },


      {


        name: `James`,

        age: `29`,

        is_premium: true,

        id: 219823



      },

      ]
    }
  },





  name: 'App',
  components: {

    SmallUserProfile

  },




}
</script>

<style></style>
