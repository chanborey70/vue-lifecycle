<template>
  <!-- team section -->
  <section class="team_section layout_padding">
    <div class="container-fluid">
      <div class="heading_container heading_center">
        <h2 class="">
          Our <span> Team</span>
        </h2>
      </div>

      <div class="team_container">
        <div class="row">
          <!-- <div class="col-lg-3 col-sm-6">
            <div class="box ">
              <div class="img-box">
                <img src="/images/team-1.jpg" class="img1" alt="">
              </div>
              <div class="detail-box">
                <h5>
                  Joseph Brown
                </h5>
                <p>
                  Marketing Head
                </p>
              </div>
              <div class="social_box">
                <a href="#">
                  <i class="fa fa-facebook" aria-hidden="true"></i>
                </a>
                <a href="#">
                  <i class="fa fa-twitter" aria-hidden="true"></i>
                </a>
                <a href="#">
                  <i class="fa fa-linkedin" aria-hidden="true"></i>
                </a>
                <a href="#">
                  <i class="fa fa-instagram" aria-hidden="true"></i>
                </a>
                <a href="#">
                  <i class="fa fa-youtube-play" aria-hidden="true"></i>
                </a>
              </div>
            </div>
          </div> -->
          <TeamCard v-for="(team,index) in teams"
          :key="index"
          :headimage="team.headimage"
          :nameheaddepartment="team.nameheaddepartment"
          :department="team.department"
          >
        </TeamCard>
        </div>
      </div>
    </div>
  </section>
  <!-- end team section -->
</template>

<script>
import TeamCard from "@/components/cards/TeamCard.vue";
export default {
components: {
    TeamCard,
},
data() {
    return {
        teams: [
            {
                headimage: "/images/team-1.jpg",
                nameheaddepartment: "Joseph Brown",
                department: "Marketing Head",
            },
            {
                headimage: "/images/team-2.jpg",
                nameheaddepartment: "Nancy White",
                department: "Marketing Head",
            },
            {
                headimage: "/images/team-3.jpg",
                nameheaddepartment: "Earl Martinez",
                department: "Marketing Head",
            },
            {
                headimage: "/images/team-4.jpg",
                nameheaddepartment: "Josephine Allard",
                department: "Marketing Head",
            },
        ],
    };
},

}
</script>
