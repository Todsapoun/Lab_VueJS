<template>
  <div>
    <br /><br />
    <h1>{{ title }}</h1>   
    <br /><br />
    <img :src="imageSrc1" alt="My Picture" style="max-width: 40%; height: auto;"/>
    <br /><br />
    <p><b>ชื่อ: </b>{{ fullName }}</p>
    <p><b>อายุ: </b>{{ age }}</p>
    <p><b>ทักษะ: </b>{{ skills }}</p>
    <br /><br />
    <img :src="imageSrc2" alt="My Picture" style="max-width: 40%; height: auto;"/>
    <p><b>อาหารที่ชอบ: </b>{{ fvfood }}</p>
    <br /><br />
    <img :src="imageSrc3" alt="My Picture" style="max-width: 40%; height: auto;"/>
    <p><b> สิ่งที่ชอบทำเวลาว่าง: </b>{{ ftime }}</p>
  </div>
</template>

<script>
export default {
  name: "MyInfo",
  data: () => ({
    title: "Personal Information",
    firstName: "Todsaporn",
    lastName: "Musipun",
    age: 22,
    skills: "JavaScript, Vue.js, HTML, CSS",
    fvfood: "Fried rice",
    ftime: "Play Game",
    imageSrc1: "https://cdn.discordapp.com/attachments/442210220517883904/1103960169290932294/Image_Me.jpg",
    imageSrc2: "https://cdn.discordapp.com/attachments/442210220517883904/1103961931284488212/resive_04062021_430x320px-2_0.webp",
    imageSrc3: "https://cdn.discordapp.com/attachments/442210220517883904/1103962524984025088/shutterstock_632848880.jpg",
  }),
  computed: {
    fullName() {
      return `${this.firstName} ${this.lastName}`;
    },
  },
};
</script>
