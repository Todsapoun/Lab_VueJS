<template>
  <div>
    <br /><br />
    <h1>{{ title }}</h1>
    <br /><br />    
    <img :src="imageSrc1" alt="My Picture" style="max-width: 40%; height: auto;"/>
    <br /><br />
    <p><b>Email: </b>{{ email }}</p>
    <p><b>เบอร์โทรศัพท์: </b>{{ telenumber }}</p>
    <p><b>ที่อยู่: </b>{{ myadd }}</p>
    <br /><br />
  </div>
</template>

<script>
export default {
  name: "MyContact",
  data: () => ({
    title: "My Contact",
    email: "musipun006@gmail.com",
    telenumber: "080-268-1330",
    myadd: "87/20 Samutprakarn",
    imageSrc1: "https://cdn.discordapp.com/attachments/442210220517883904/1103965445037502474/t.jpg",
  }),
};
</script>
