<template>
  <div>
    <br /><br />
    <h1>{{ title }}</h1>    
    <br /><br />
    <img :src="imageSrc1" alt="My Picture" style="max-width: 40%; height: auto;"/>
    <br /><br />
    <p><b>ผลงานที่เคยทำ: </b>{{ mywork }}</p>
    <p><b>สิ่งที่สนใจ: </b>{{ interests }}</p>
    <br /><br />
  </div>
</template>

<script>
export default {
  name: "MyProject",
  data: () => ({
    title: "Project Information",
    mywork: "Book Store Application",
    interests: "Doing Something New",
    imageSrc1: "https://media.discordapp.net/attachments/442210220517883904/1103970072973819955/f3c09992a3593c04.jpg?width=450&height=450",
  }),
};
</script>
