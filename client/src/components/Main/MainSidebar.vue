<template>
  <section id="sidebar">
    <div class="core-block">
      <router-link to="/today">
        <i class="fas fa-tasks"></i><p>Сегодня</p>
<!--        <span></span>-->
      </router-link>

      <router-link to="/upcoming">
        <i class="fa fa-calendar"></i><p>Предстоящее</p>
<!--        <span></span>-->
      </router-link>

      <router-link to="/archive">
          <i class="fa fa-calendar-times"></i><p>Архив</p>
<!--        <span></span>-->
      </router-link>

      <router-link to="/expired">
          <i class="fa fa-clock"></i><p>Просроченное</p>
<!--        <span></span>-->
      </router-link>
    </div>
  </section>
</template>

<script>
export default {
  name: "MainSidebar",
  data(){
    return{
      // todayCount: 0,
      // upcomingCount: 0,
      // archiveCount: 0
    }
  }
}
</script>

<style scoped lang="scss">
#sidebar {
  position: sticky;
  top: 20px;
  margin: 0 40px 0 35%;
  border: 2px solid #90A5E6;
  border-radius: 12px;
  max-height: 175px
}
.core-block {
  display: flex;
  z-index: 0;
  text-align: left;
  justify-content: space-between;
  align-items: flex-start;
  padding: 0 1em;
  flex-direction: column;
  margin-right: 5px;
  color: black;
    a{
      padding: 8px 0;
      text-align: left;
      margin-top: .3em;
      text-decoration: none;
      font-size: 1em;
      color: black;
      display: flex;
      justify-content: space-between;
      i{
        padding-right: .5em;
        padding-top: .25em;
        margin-right: .4em;
      }
      span{
        padding-left: .3em;
      }
      p {
        text-align: left;
      }
    }
    a:last-child {
      margin-bottom: .5em;
    }
    a:hover{
      background: rgba(173,216,230,0.3);
    }

}

</style>