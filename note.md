* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  text-decoration: none;
  color: black;
}

body {
  background: #dbdbdb;
}

.navbar {
  display: flex;
  justify-content: space-between;
  margin: 30px;
}

.Top {
  background: #dbdbdb;
  border-radius: 10%;
  width: 100%;
}
h1 {
  text-align: center;
}

.btn_1 {
  width: 80px;
  height: 40px;
  border: none;
  border-radius: 20px;
  text-wrap: wrap;
}

.btn_1:hover {
  cursor: pointer;
  color: whitesmoke;
  background: gray;
}

.nav_left {
  display: flex;
  align-items: center;
  gap: 15px;
}

.nav_right {
  display: flex;
  gap: 12px;
  align-items: center;
}

a:hover {
  color: blue;
  text-decoration: underline;
}

.profile {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
}

.profile_content {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 40%;
  text-align: center;
  gap: 30px;
  margin-bottom: 50px;
}

.pic {
  border-radius: 50%;
  width: 25%;
  border: 5px solid white;
  box-shadow: rgba(0, 0, 0, 0.2) 0px 60px 40px -7px;
}

.name {
  border: none;
  border-radius: 20px;
  width: 8%;
  height: 32px;
  position: absolute;
  transform: translate(130px, -80px);
  rotate: 350deg;
  background: whitesmoke;
  box-shadow: rgba(60, 64, 67, 0.3) 0px 1px 2px 0px,
    rgba(60, 64, 67, 0.15) 0px 2px 6px 2px;
}

.btn_2 {
  background: #000;
  color: whitesmoke;
  width: 10em;
  height: 40px;
  text-align: center;
  border-radius: 20px;
  font-size: x-small;
}

.btn_2:hover {
  scale: 1.2;
  color: gold;
  cursor: pointer;
  transition: 0.3s ease-in;
}

#icon {
  width: 10%;
  height: 30px;
  filter: brightness(100%) saturate(0);
}

#icon:hover {
  transform: scale(1.2);
  transition: 0.3s ease-in;
  cursor: pointer;
  filter: brightness(100%) saturate(100%);
}
.main {
  background: whitesmoke;
  border-radius: 10%;
  width: 100%;
  position: relative;
}

.center {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 50px;
  padding: 20px;
  margin: 20px;
  height: 12em;
}

.Bottom {
  text-align: center;
  position: relative;
  top: 50px;
}

.Bottom hr {
  width: 70%;
  margin-top: 70px;
  margin-left: 15%;
  color: gray;
}

.btn_3 {
  border: none;
  border-radius: 15px;
  width: 8%;
  background: whitesmoke;
  height: 25px;
  position: relative;
  transform: translate(0px, -15px);
  rotate: 352deg;
}

.footer {
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 60px 15% 100px;
  gap: 40px;
}

.footer img {
  width: 30px;
}

.footer-flex {
  display: flex;
  flex-direction: column;
  gap: 20px;
  width: 100%;
}

@media (max-width: 480px) {
  body {
    overflow-x: hidden;
    background: #dbdbdb;
  }

  /* --- Navbar --- */
  .navbar {
    flex-direction: column;
    align-items: center;
    margin: 10px;
    text-align: center;
    gap: 8px;
  }

  .nav_left,
  .nav_right {
    flex-direction: column;
    align-items: center;
    gap: 6px;
  }

  .btn_1 {
    display: none;
  }

  /* --- Profile Section --- */
  .profile {
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 10px 0;
  }

  .profile_content {
    width: 95%;
    gap: 15px;
    margin-bottom: 20px;
  }

  .profile_content h1 {
    font-size: 1.2em;
    line-height: 1.3;
    text-align: center;
    padding: 0 10px;
  }

  .pic {
    width: 65%;
    border: 3px solid white;
  }

  .name {
    display: none;
  }

  .btn_2 {
    width: 85%;
    max-width: 220px;
    font-size: 0.9em;
    height: 40px;
    border-radius: 25px;
  }

  #icon {
    width: 26px;
    height: 26px;
  }

  /* --- Main / Center Section --- */
  .main {
    width: 100%;
    border-radius: 0;
  }

  .center {
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 15px;
    height: auto;
    padding: 10px;
    margin: 10px 0;
  }

  .center img {
    width: 85%;
    max-width: 260px;
  }

  /* --- Bottom Section --- */
  .Bottom {
    top: 15px;
    text-align: center;
  }

  .Bottom hr {
    width: 90%;
    margin: 25px auto;
  }

  .btn_3 {
    display: none;
  }

  /* --- Footer --- */
  .footer {
    flex-direction: column;
    align-items: center;
    margin: 30px 5%;
    gap: 15px;
  }

  .footer-flex {
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
    gap: 10px;
  }

  .footer img {
    width: 22px;
  }

  /* --- Text scaling for mobile readability --- */
  h1, h2, h3, p, a {
    font-size: 0.95em;
  }

  /* Keep the learn more button prominent */
  .btn_2:hover {
    scale: 1.05;
    transition: 0.2s ease-in;
  }
}