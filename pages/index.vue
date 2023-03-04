<template>
  <div class="home">
    <!-- LANDING -->
    <div class="site-container py-10 lg:pb-36">
      <div class="home--landing">
        <div class="home--landing__container home--landing__left">
          <h1 class="home--landing__container--title">
            Decision Support Model
          </h1>
          <p class="home--landing__container--subtitle">
            DSM is a model that can provide problem-solving or decision support
            used by organizations, individuals, companies, and others to get
            maximum decisions.
          </p>
        </div>
        <div class="home--landing__container">
          <img
            src="@/assets/img/static/home/landing-2.png"
            alt="Image Landing"
            class="home--landing__container--img"
          />
        </div>
      </div>
    </div>
    <!-- PORTFOLIO -->
    <div class="site-container pb-20 lg:pb-36">
      <div class="home--portfolio">
        <h1 class="home--portfolio__title">Our Portfolio</h1>
        <p class="home--portfolio__subtitle">
          Checkout our latest portfolio of Decision Support Model
        </p>

        <div class="home--portfolio__container">
          <div
            v-for="(item, i) in portfolios"
            :key="`portfolio-${i}`"
            class="home--portfolio__container--wrapper"
          >
            <CardPortfolio :item="item" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "IndexPage",
  layout: "default",
  data() {
    return {
      pwr: [
        {
          title: "Project Plan",
          subtitle:
            "There are many variations of the passages of lorem Ipsum from available, majority.",
          link: "",
        },
        {
          title: "Interior Work",
          subtitle:
            "There are many variations of the passages of lorem Ipsum from available, majority. There are many variations of the passages",
          link: "",
        },
        {
          title: "Realization",
          subtitle:
            "There are many variations of the passages of lorem Ipsum from available, majority.",
          link: "",
        },
      ],
      wtpt: [
        {
          photo: "",
          name: "Nattasha Mith",
          region: "New York, USA",
          comment:
            "Lorem Ipsum is simply dummy text of the typesetting industry. Ipsum has been.",
        },
        {
          photo: "",
          name: "Raymond Galario",
          region: "Sydney, Australia",
          comment:
            "Lorem Ipsum is simply dummy text of the typesetting industry. Ipsum has been scrambled it to make a type book.",
        },
        {
          photo: "",
          name: "Benny Roll",
          region: "Jakarta, Indonesia",
          comment:
            "Lorem Ipsum is simply dummy text of the typesetting industry. Ipsum has been scrambled.",
        },
      ],
      projects: [
        {
          title: "Modern Kitchen",
          desc: "Decor / Artchitecture",
        },
        {
          title: "Cozy Living Room",
          desc: "Design / Artchitecture",
        },
        {
          title: "Cozy Working Room",
          desc: "Design / Artchitecture",
        },
        {
          title: "Modern Playground",
          desc: "Decor / Artchitecture",
        },
      ],
      points: [
        {
          count: 12,
          label: "Year Of Experience",
        },
        {
          count: 85,
          label: "Success Project",
        },
        {
          count: 15,
          label: "Active Project",
        },
        {
          count: 95,
          label: "Happy Customers",
        },
      ],
      portfolios: [
        {
          id: "1",
          img: ["portfolio-1.png", "portfolio-2.png"],
          title:
            "Decision Support Model Based on Fuzzy Logic To Determine Employee Salary",
          author: "Gregoryus Imannuel Perdana",
          date: "26 December, 2022",
          tag: "Multistage Fuzzy Logic",
        },
        {
          id: "2",
          img: ["portfolio-2.png"],
          title:
            "Decision Support Model Based on Fuzzy Logic To Determine Employee Salary",
          author: "Gregoryus Imannuel Perdana",
          date: "22 December, 2022",
          tag: "Fuzzy AHP",
        },
        {
          id: "3",
          img: ["portfolio-1.png", "portfolio-2.png"],
          title:
            "Decision Support Model Based on Fuzzy Logic To Determine Employee Salary",
          author: "Gregoryus Imannuel Perdana",
          date: "25 December, 2022",
          tag: "Fuzzy Guzzy",
        },
      ],
    };
  },
};
</script>
