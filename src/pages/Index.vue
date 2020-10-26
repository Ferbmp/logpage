<template>
  <q-page padding>
    <header>
        <h3>White Label</h3>
    </header>

    <div class="content-all">

        <section class="form">
            <section class="title">
                <h3>Crie Sua Conta</h3>
                <i class="material-icons" id="btnFace"> facebook </i>

            </section>
            <form id="register" action="post">

                <div class="item">
                    <input type="text" name="Nome" id="" placeholder="Nome">
                </div>

                <div class="item">
                    <input type="text" name="CPF/CNPJ" id="" placeholder="CPF/CNPJ">
                </div>

                <div class="item">
                    <input type="text" name="Cel" id="" placeholder="CEL">
                </div>

                <div class="item">
                    <input type="text" name="CEP" id="" placeholder="CEP">
                </div>

                <div class="item">
                    <input type="password" name="password" id="" placeholder="Digite sua Senha">
                </div>

                <div class="item">
                    <input type="password" name="password" id="" placeholder="Repita a senha">
                </div>

            </form>
        </section>

        <section class="documents">
            <div class="content-cards">
                <div class="card">
                    <i class="material-icons" id="btnCamera"> camera_alt </i>
                    <h2>Anexe Sua Foto</h2>
                </div>
            </div>

            <div class="content-cards">
                <div class="card">
                    <i class="material-icons" id="btnDoc"> post_add </i>
                    
                    <h2>  Anexe um Documento  </h2>
                    <p>(CNH, CNPJ ou RG)</p>
                </div>
            </div>

        </section>


    </div>

    <section class="grid-footer">
        <section class="footer">

            <div>
                <input type="checkbox" id="confirm">
                <label for="confirm">TODOS OS DADOS ENTRARAM EM ANÁLISE, CASO ESTEJA DE ACORDO <a
                        href="/style.css">ACEITE OS TERMOS DE USO</a> </label>
            </div>

            <div>
                <button class="button" type="submit" form="register" value="Submit">Confirmar</button>
            </div>


        </section>
    </section>

  </q-page>
</template>

<script>
export default {
  data (){
    return{
      message: 'I love Vue.js so hard'
    }
  },
  methods: {
    clearMessage(){
      this.message = ''
    },
    alertMessage(){
      alert(this.message)
    }
  }
}
</script>

<style >
  @import url('https://fonts.googleapis.com/css2?family=Source+Sans+Pro&display=swap');

body{
    background-color: black;
    font-family: 'Source Sans Pro', sans-serif;
}

header{

}

h3{
    color: white;
    font-size: 18px;
    font-weight: bold;
}

title{
    letter-spacing: 3px;
}

.content-all{
    width: auto;
    height: max-content;
    margin-top: 44px;
    display: grid;
    grid-template-columns: 1fr 1fr;
    margin-left: 40px;
}

.title{
    padding: 4px;
    display: flex;

}

#btnFace{
    color: white;
    font-size: 24px;
    padding: 20px;
}

form{
    padding: 4px;
}

.form .item{
    padding: 4px;
    display: grid;
    grid-template-columns: 500px;
    border: 4px solid;
}

.form input{
    border: 8px solid white;
    border-radius: 8px ;
}


.form h3{
    color: white;
}

header{
    text-align: center;   
}



  .documents{
      display: grid;
      grid-template-columns: 1fr 1fr;
      align-items: center;
      justify-content: space-between;
  }

  #btnCamera {
      font-size: 45px;
 }

 #btnDoc {
     font-size: 45px;
 }

 p{
     color: grey;
     font-weight: bold;
 }

  .content-cards{
      display: flex;
      justify-content: center;
      align-items: center;
      align-content: center;
      width: 300px;
      height: 300px;
      background: white;
      border-radius: 20px;
      text-align: center;
      padding-top: 0px;
      margin-top: 62px;
  }
 
  .card a {
      text-decoration: none;
  }
  .footer{
     padding-top: 20px;
     padding-left: 50px;
     padding-right: 50px;
     display: flex;
     justify-content: space-between;
     align-items: center;
  }

  .button{
     background-color: #79d1ff;
     border: 4px solid #79d1ff;
     border-radius: 24px;
     width: 300px;
     height: auto;
     text-align: center;
     font-size: 20px;
     font-family: 'Source Sans Pro', sans-serif;
     color: white;
     font-weight: bold;
     
  }

  .footer label{
    color: white;
  }

  a{
      text-decoration: none;
  }

  section.documents{
      /* padding-top: 112px; */
  }

  h2{
    font-size: 24px;
    font-weight: bold;
    line-height: 2px;
  }

  div label{
    padding-left: 8px;
  }
</style>
