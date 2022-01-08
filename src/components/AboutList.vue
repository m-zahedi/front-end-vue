<template>

<body>
  <div class="profile-card">
    <div class="card-header">
      <div class="pic">

      </div>
      <div class="name">Milad Zahediyami</div>
      <div class="desc">CPS2 M2</div>
      <div class="sm">
        <a href="#" class="fab fa-facebook-f"></a>
        <a href="#" class="fab fa-twitter"></a>
        <a href="#" class="fab fa-github"></a>
        <a href="#" class="fab fa-youtube"></a>
      </div>
      <a href="https://github.com/m-zahedi/" class="contact-btn">Github</a>

    </div>
    <div class="card-footer">
      <div class="numbers">
        <div class="item">
          <span>120</span>
          Posts
        </div>
        <div class="border"></div>
        <div class="item">
          <span>127</span>
          Following
        </div>
        <div class="border"></div>
        <div class="item">
          <span>120</span>
          Followers
        </div>
      </div>
    </div>
  </div>
</body>
</template>


<script>

export default {
    name: 'AboutList'
}
</script>

<style scoped>
*{
  margin: 0;
  padding: 0;
  font-family: "Ubuntu", sans-serif;
  box-sizing: border-box;
  text-decoration: none;
}

body{
  height: 100vh;

  background-size: cover;
  display: flex;
  align-items: center;
  justify-content: center;
}

.profile-card{
  width: 400px;
  text-align: center;
  border-radius: 8px;
  overflow: hidden;
}

.card-header{
  background: #16a085;
  padding: 60px 40px;
}

.pic{
  display: inline-block;
  padding: 8px;
  background: linear-gradient(130deg, #74b9ff, #e66767);
  margin: auto;
  border-radius: 50%;
  background-size: 200% 200%;
  animation: animated-gradient 2s linear infinite;
}

@keyframes animated-gradient{
  25%{
    background-position: left bottom;
  }
  50%{
    background-position: right bottom;
  }
  75%{
    background-position: right top;
  }
  100%{
    background-position: left top;
  }
}



.name{
  color: #f2f2f2;
  font-size: 28px;
  font-weight: 600;
  margin: 10px 0;
}

.desc{
  font-size: 18px;
  color: white;
}

.sm{
  display: flex;
  justify-content: center;
  margin: 20px 0;
}

.sm a{
  color: #f2f2f2;
  width: 56px;
  font-size: 22px;
  transition: .3s linear;
}

.sm a:hover{
  color: #e66767;
}

.contact-btn{
  display: inline-block;
  padding: 12px 50px;
  color: white;
  border: 2px solid white;
  border-radius: 6px;
  margin-top: 16px;
  transition: .3s linear;
}

.contact-btn:hover{
  background: #3a8a62;
  color: #f2f2f2;
}

.card-footer{
  background: #f4f4f4;
  padding: 60px 10px;
}

.numbers{
  display: flex;
  align-items: center;
}

.item{
  flex: 1;
  text-transform: uppercase;
  font-size: 13px;
  color: #30ad2b;
}

.item span{
  display: block;
  color: #19be5e;
  font-size: 30px;
}

.border{
  width: 1px;
  height: 30px;
  background: #bbb;
}


</style>