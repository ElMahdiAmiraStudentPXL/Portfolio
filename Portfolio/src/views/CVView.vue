<template>
    <div class="container">
        <header class="header">
        </header>

        <main class="content">
            <section class="intro-section">
                <img class="profile-photo" src="../assets/profielfoto.jpg" alt="Profile Photo">
                <div class="intro-text">
                    <h2>Introductie</h2>
                    <p>
                        Hallo, ik ben El Mahdi Amira. Ik ben iemand die al zijn hele leven lang een passie heeft voor technologie.
                        Mijn huidige studie is graduaat in het programmeren aan de PXL in Hasselt. Hier beneden vindt u mijn vorige werkervaringen,
                        taalvaardigheden en behaalde diploma's.
                    </p>
                </div>
            </section>

            <section class="skills-section">
                <h2>Taalvaardigheden</h2>
                <table class="skills-table">
                    <tr>
                        <th>Nederlands:</th>
                        <td>10/10</td>
                    </tr>
                    <tr>
                        <th>Frans:</th>
                        <td>7/10</td>
                    </tr>
                    <tr>
                        <th>Engels:</th>
                        <td>9/10</td>
                    </tr>
                    <tr>
                        <th>Duits:</th>
                        <td>4/10</td>
                    </tr>
                </table>
            </section>

            <section class="education-section">
                <h2>Diploma's</h2>
                <table class="education-table">
                    <tr>
                        <th>Getuigschrift A 1ste graad Secundair onderwijs Latijn Stedelijke Humaniora</th>
                        <td>2016</td>
                    </tr>
                    <tr>
                        <th>Getuigschrift ASO 2de graad Secundair onderwijs Economie Stedelijke Humaniora</th>
                        <td>2018</td>
                    </tr>
                    <tr>
                        <th>Diploma ASO 3de graad Secundair onderwijs Economie-moderne talen Stedelijke Humaniora</th>
                        <td>2020</td>
                    </tr>
                </table>
            </section>

            <section class="experience-section">
                <h2>Werkervaringen</h2>
                <ul>
                    <li>Gewerkt bij Carrefour in de M2.</li>
                    <li>
                        Regelmatig gewerkt bij Plukon van 08/2019 tot 12/2021 tijdens vakantieperiodes.
                    </li>
                    <li>Huidige job: jobstudent bij Albert Heijn in Lanaken</li>
                </ul>
            </section>
        </main>
    </div>
</template>

<script>
export default {
    data() {
        return {
            isMenuOpen: false,
        };
    },
    methods: {
        toggleMenu() {
            this.isMenuOpen = !this.isMenuOpen;
        },
    },
};
</script>

<style lang="scss" scoped>

.container {
  max-width: 960px;
  margin: 0 auto;
  padding: 20px;
}

.header {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.title {
  font-family: 'Roboto', Arial, sans-serif;
  font-size: 32px;
}

.navbar-toggle {
  display: none;
}

.navbar-menu {
  list-style: none;
  display: flex;
}

.navbar-menu li {
  margin-left: 20px;
}

.navbar-menu li a {
  color: #333;
  text-decoration: none;
}

.navbar-menu.active {
  display: block;
}

.icon-bar {
  display: block;
  width: 20px;
  height: 2px;
  background-color: #333;
  margin-bottom: 4px;
}

.content {
  margin-top: 20px;
}

.intro-section {
  display: flex;
  align-items: center;
}

.profile-photo {
  width: 200px;
  height: auto;
  margin-right: 20px;
  border: 2px solid #333;
  border-radius: 50%;
}

.intro-text {
  font-family: 'Roboto', Arial, sans-serif;
}

.skills-section {
  margin-top: 40px;
}

.skills-table {
  width: 100%;
  font-family: 'Roboto', Arial, sans-serif;

  th {
    text-align: left;
    padding-right: 10px;
  }
}

.education-section {
  margin-top: 40px;
}

.education-table {
  width: 100%;
  font-family: 'Roboto', Arial, sans-serif;

  th {
    text-align: left;
    padding-right: 10px;
  }
}

.experience-section {
  margin-top: 40px;
}

.experience-section ul {
  list-style: disc;
  padding-left: 20px;
}

@media screen and (max-width: 768px) {
  .navbar-toggle {
    display: block;
    background: none;
    border: none;
    cursor: pointer;
    padding: 10px;
  }

  .navbar-toggle:focus {
    outline: none;
  }

  .navbar-toggle:hover .icon-bar {
    background-color: #999;
  }

  .navbar-menu {
    display: none;
    position: absolute;
    top: 100%;
    left: 0;
    width: 100%;
    background-color: #f9f9f9;
    padding: 10px;
  }

  .navbar-menu li {
    margin-left: 0;
    margin-bottom: 10px;
  }

  .navbar-menu.active {
    display: block;
  }
}

@media screen and (max-width: 480px) {
  .container {
    padding: 10px;
  }

  .title {
    font-size: 24px;
  }

  .profile-photo {
    width: 150px;
    height: auto;
  }
}
</style>
