<script>
  import Header from "../components/Header.svelte";
  import Main from "../components/Main.svelte";
  import Sidebar from "../components/Sidebar.svelte";
  import TimeLine from "../components/TimeLine.svelte";

  let data = {
    user: { nickname: "matthewdrf", name: "Matthew Rosell" },
    posts: [
      {
        username: "matthewdrf",
        location: "Lima, Peru",
        avatar:
          "https://www.discordianos.com/uploads/monthly_2020_07/fotopelelaperfil.jpg.384d7c7d3bb5f4a52983b5bc0aad212c.jpg",
        photo: "https://arepa.s3.amazonaws.com/elmo002.jpg",
        like: false,
        bookmark: false,
        postComment: "Disfrutando de mi piscina",
        comments: [
          { id: 123234535, text: "Hola Elmo", username: "Crispeta" },
          { id: 1232322312, text: "¡Hola!", username: "Dollarsin" },
        ],
      },
      {
        username: "matthewdrf",
        location: "Lima, Peru",
        avatar:
          "https://www.discordianos.com/uploads/monthly_2020_07/fotopelelaperfil.jpg.384d7c7d3bb5f4a52983b5bc0aad212c.jpg",
        photo: "https://arepa.s3.amazonaws.com/elmo001.jpeg",
        like: false,
        bookmark: false,
        postComment: "Hola...",
        comments: [{ id: 123234535, text: "Elmito", username: "gndx" }],
      },
      {
        username: "matthewdrf",
        location: "Lima, Peru",
        avatar:
          "https://www.discordianos.com/uploads/monthly_2020_07/fotopelelaperfil.jpg.384d7c7d3bb5f4a52983b5bc0aad212c.jpg",
        photo: "https://arepa.s3.amazonaws.com/elmo003.jpg",
        like: false,
        bookmark: false,
        postComment: "Un dia feliz",
        comments: [],
      },
      {
        username: "matthewdrf",
        location: "Lima, Peru",
        avatar:
          "https://www.discordianos.com/uploads/monthly_2020_07/fotopelelaperfil.jpg.384d7c7d3bb5f4a52983b5bc0aad212c.jpg",
        photo: "https://arepa.s3.amazonaws.com/elmo004.jpg",
        like: false,
        bookmark: false,
        postComment: "Un hueso para la dieta",
        comments: [],
      },
      {
        username: "matthewdrf",
        location: "Lima, Peru",
        avatar:
          "https://www.discordianos.com/uploads/monthly_2020_07/fotopelelaperfil.jpg.384d7c7d3bb5f4a52983b5bc0aad212c.jpg",
        photo: "https://arepa.s3.amazonaws.com/elmo005.jpg",
        like: false,
        bookmark: false,
        postComment: "Conociendo el vencindario",
        comments: [],
      },
      {
        username: "matthewdrf",
        location: "Lima, Peru",
        avatar:
          "https://www.discordianos.com/uploads/monthly_2020_07/fotopelelaperfil.jpg.384d7c7d3bb5f4a52983b5bc0aad212c.jpg",
        photo: "https://arepa.s3.amazonaws.com/elmo006.jpg",
        like: false,
        bookmark: false,
        postComment: "I Love JS",
        comments: [],
      },
      {
        username: "matthewdrf",
        location: "Lima, Peru",
        avatar:
          "https://www.discordianos.com/uploads/monthly_2020_07/fotopelelaperfil.jpg.384d7c7d3bb5f4a52983b5bc0aad212c.jpg",
        photo: "https://arepa.s3.amazonaws.com/elmo007.png",
        like: false,
        bookmark: false,
        postComment: "A dormir",
        comments: [],
      },
      {
        username: "matthewdrf",
        location: "Lima, Peru",
        avatar:
          "https://www.discordianos.com/uploads/monthly_2020_07/fotopelelaperfil.jpg.384d7c7d3bb5f4a52983b5bc0aad212c.jpg",
        photo: "https://arepa.s3.amazonaws.com/elmo008.png",
        like: false,
        bookmark: false,
        postComment: "Hola, ¿Cómo te llamas?",
        comments: [],
      },
      {
        username: "matthewdrf",
        location: "Lima, Peru",
        avatar:
          "https://www.discordianos.com/uploads/monthly_2020_07/fotopelelaperfil.jpg.384d7c7d3bb5f4a52983b5bc0aad212c.jpg",
        photo: "https://arepa.s3.amazonaws.com/elmo009.png",
        like: false,
        bookmark: false,
        postComment: "Dia de fogata",
        comments: [],
      },
    ],
  };
</script>

<style>
  @import url("https://fonts.googleapis.com/css2?family=Lato:wght@300;400&family=Pacifico&display=swap");

  :global(body) {
    background-color: #fafafa;
    color: rgba(38, 38, 38, 0.7);
    font-family: "Lato", sans-serif;
    margin: 0;
    padding: 0;
  }

  :global(h1, h2, h3) {
    margin: 0;
    padding: 0;
  }
</style>

<Header />
<Main>
  <TimeLine posts={data.posts} />
  <Sidebar {...data.user} />
</Main>
