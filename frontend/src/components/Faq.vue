<template>
  <div>
    <!-- breadcrumb start -->
    <div class="breadcrumb-container">
      <div class="container">
        <ol class="breadcrumb">
          <li><i class="fa fa-home pr-10"></i><a href="home">Accueil</a></li>
          <li class="active">FAQ</li>
        </ol>
      </div>
    </div>
    <!-- breadcrumb end -->
    <!-- section -->
    <section class="main-container">
      <div class="container">
        <div class="row">
          <!-- section start -->
          <section class="dark-translucent-bg" style="background-image:url(assets/images/poignee_de_main.jpg); background-position: 50% 50%">
            <div class="container">
              <div class="row justify-content-lg-center">
                <div class="col-lg-12">
                  <h2 class="text-center mt-4">
                    <div><span class="bold_6">Achetez</span> en confiance un <span class="bold_6">véhicule d'occasion</span></div>
                  </h2>
                  <div class="separator with-icon"><i class="fa fa-car bordered"></i></div>
                </div>
              </div>
            </div>
          </section>
          <!-- section end -->
          <!-- debut image fixe
          <div class="col-md-12"> <img src="assets/images/corporate-1-slider-slide-2.jpg" class="img-responsive" alt="slidebg2" data-bgposition="center top" data-bgrepeat="no-repeat" data-bgfit="cover"></div>
    <!-- fin image fixe -->
        </div>
      </div>
    </section>
    <!-- section -->
    <!-- main-container start -->
    <section class="main-container">
      <div class="container">
        <div class="row">
          <!-- main start -->
          <div class="main col-md-12">
            <!-- page-title start -->
            <h3 class="title"><span class="text-defaut">F</span>AQ</h3>
            <div class="separator-2"></div>
            <!-- page-title end -->
          </div>
          <!-- main end -->
        </div>
      </div>
    </section>
    <div class="container">
      <div class="row">
        <div class="col-lg-12 mb-20">
          <p>Voici les questions les plus fréquemment posées. Si vous ne trouvez pas dans cette liste la réponse à votre interrogation, <a :href="'mailto:histovec@interieur.gouv.fr?subject=Question%20FAQ'">contactez-nous</a></p>
          <!-- accordion start -->
          <!-- ================ -->
          <div class="panel-group collapse-style-2" id="accordion-2">
            <!-- debut question 1 -->
            <div class="panel panel-default">
              <div class="panel-heading">
                <h4 class="panel-title"> <a @click="choose('a')" class="clickable" :class="[{'collapsed' : choice != 'a'}]"> <i class="fa fa-file-text-o pr-10"></i>Comment utiliser HistoVec ? </a> </h4>
              </div>
              <div class="panel-collapse collapse" :class="[{'in' : choice === 'a'}]">
                <div class="panel-body">
                 <DL><DT>Vous êtes vendeur :</DT>
     						 <DD><OL><LI>sur la page vendeur, remplissez le formulaire pour vous identifier avec les informations demandées, et validez.
     						 <UL>Note : s’il s’agit d’un véhicule d’entreprise, cliquez sur l’onglet “Entreprise”</UL></LI>
     						<LI>le rapport du véhicule est affiché. Vous pouvez consulter les différentes sections sur le menu de gauche.</LI>
     						<LI>vous pouvez transmettre le lien vers le rapport à un tiers en cliquant sur le menu “Transmettre le rapport”.</LI></OL></DD>
     						<DT>Vous êtes acheteur :</DT>
     						<DD><UL>Demandez au vendeur de vous transmettre le lien vers le rapport en le générant sur le site Histovec.</UL></DD>
     						</DL>
     						</div>
              </div>
            </div>
            <!-- fin question 1 -->
            <!-- debut question 2 -->
            <div class="panel panel-default">
              <div class="panel-heading">
                <h4 class="panel-title"> <a @click="choose('b')" class="clickable" :class="[{'collapsed' : choice !== 'b' }]"> <i class="fa fa-file-text-o pr-10"></i>Comment retrouver mon rapport HistoVec ultérieurement ?</a> </h4>
              </div>
              <div class="panel-collapse collapse" :class="[{'in' : choice === 'b'}]">
                <div class="panel-body">
                  <UL>Le rapport généré est consultable pendant une période de 4 semaines aprés sa génération, grâce au lien qui a été fourni par le vendeur.</UL>
                </div>
              </div>
            </div>
            <!-- fin question 2 -->
            <!-- debut question 3 -->
            <div class="panel panel-default">
              <div class="panel-heading">
                <h4 class="panel-title"> <a @click="choose('c')" class="clickable" :class="[{'collapsed' : choice !== 'c' }]"> <i class="fa fa-file-text-o pr-10"></i>A qui s’adresse HistoVec ?</a> </h4>
              </div>
              <div class="panel-collapse collapse" :class="[{'in' : choice === 'c'}]">
                <div class="panel-body">
                  <DL><DT>Je vends mon véhicule d’occasion :</DT>
                      <DD><UL>HistoVec vous permet de valoriser votre offre en fournissant gratuitement un rapport d’historique officiel qui rassurera vos acheteurs potentiels.</UL></DD>
                      <DT>J’achète un véhicule d’occasion :</DT>
                      <DD><UL>HistoVec vous permet de vous informer, de faire un choix éclairé sur les véhicules sélectionnés et d’éviter les mauvaises surprises.</UL></DD>
                      <DT>Je suis un professionnel négociant automobile :</DT>
                      <DD><UL>Fiabilisez et valorisez votre stock de véhicules d’occasion en permettant à votre entreprise et vos clients de vérifier l’historique des véhicules acquis.</UL></DD>
    	                <DT>Je loue ma voiture à des particuliers :</DT>
                      <DD><UL>Je peux rassurer mes clients potentiels en fournissant gratuitement un historique officiel du véhicule.</UL></DD>
                  </DL>
                </div>
              </div>
            </div>
            <!-- fin question 3 -->
            <!-- debut question 4 -->
            <div class="panel panel-default">
              <div class="panel-heading">
                <h4 class="panel-title"> <a @click="choose('d')" class="clickable" :class="[{'collapsed' : choice !== 'd' }]"> <i class="fa fa-file-text-o pr-10"></i>D’où proviennent les informations d’HistoVec ?</a> </h4>
              </div>
              <div class="panel-collapse collapse" :class="[{'in' : choice === 'd'}]">
                <div class="panel-body">
                  <UL>Les informations du rapport sont issues du système d’immatriculation des véhicules (SIV) du ministère de l’intérieur.</UL>
                </div>
              </div>
            </div>
            <!-- fin question 4 -->
            <!-- debut question 5 -->
            <div class="panel panel-default">
              <div class="panel-heading">
                <h4 class="panel-title"> <a @click="choose('e')" class="clickable" :class="[{'collapsed' : choice !== 'e' }]"> <i class="fa fa-file-text-o pr-10"></i>Comment consulter le rapport d’un véhicule qui ne m’appartient pas ?</a> </h4>
              </div>
              <div class="panel-collapse collapse" :class="[{'in' : choice === 'e'}]">
                <div class="panel-body">
                  <UL>Seul le propriétaire du certificat d’immatriculation peut générer le rapport HistoVec de son véhicule, qu’il choisit de transmettre à des tiers.</UL>
                </div>
              </div>
            </div>
            <!-- fin question 5 -->
            <!-- debut question 6 -->
            <div class="panel panel-default">
              <div class="panel-heading">
                <h4 class="panel-title"> <a @click="choose('f')" class="clickable" :class="[{'collapsed' : choice !== 'f' }]"> <i class="fa fa-file-text-o pr-10"></i>Quelles sont les garanties d’HistoVec ?</a> </h4>
              </div>
              <div class="panel-collapse collapse" :class="[{'in' : choice === 'f'}]">
                <div class="panel-body">
                  <DL><DT>Officiel :</DT>
                      <DD><UL>HistoVec est un site produit par le ministère de l’intérieur et fournit les données du système d’immatriculation des véhicules (SIV).</UL></DD>
                      <DT>Confidentiel :</DT>
                      <DD><UL>Seul le propriétaire du certificat d’immatriculation peut générer le rapport HistoVec de son véhicule, qu’il choisit de transmettre à des tiers. </UL></DD>
                      <DT>Gratuit : </DT>
                      <DD><UL>HistoVec est entièrement gratuit pour les vendeurs et les acheteurs. Il s’agit d’un service public pour contribuer à la sécurisation des transactions de véhicules d’occasion. </UL></DD>
                  </DL>
                </div>
              </div>
            </div>
            <!-- fin question 6 -->
            <!-- debut question 7 -->
            <div class="panel panel-default">
              <div class="panel-heading">
                <h4 class="panel-title"> <a @click="choose('g')" class="clickable" :class="[{'collapsed' : choice !== 'g' }]"> <i class="fa fa-file-text-o pr-10"></i>Est-ce que les informations sont complètes ?</a> </h4>
              </div>
              <div class="panel-collapse collapse" :class="[{'in' : choice === 'g'}]">
                <div class="panel-body">
                  <UL>Seules les informations connues du Ministère de l’Intérieur sont fournies. Par exemple, ne sont enregistrés que les sinistres déclarés à l’assureur et pour lesquels un expert a enregistré une procédure VRC (Véhicule à Réparation Contrôlée).</UL>
                </div>
              </div>
            </div>
            <!-- fin question 7 -->
            <!-- debut question8 -->
            <div class="panel panel-default">
              <div class="panel-heading">
                <h4 class="panel-title"> <a @click="choose('h')" class="clickable" :class="[{'collapsed' : choice !== 'h' }]"> <i class="fa fa-file-text-o pr-10"></i>Comment signaler une information manquante ou inexacte ?</a> </h4>
              </div>
              <div class="panel-collapse collapse" :class="[{'in' : choice === 'h'}]">
                <div class="panel-body">
                  <UL><a :href="'mailto:histovec@interieur.gouv.fr?subject=Signaler%20une%20erreur'">contactez-nous</a></UL>
                </div>
              </div>
            </div>
            <!-- fin question 9 -->
            <!-- debut question 9 -->
            <div class="panel panel-default">
              <div class="panel-heading">
                <h4 class="panel-title"> <a @click="choose('i')" class="clickable" :class="[{'collapsed' : choice !== 'i' }]"> <i class="fa fa-file-text-o pr-10"></i>Je ne trouve pas mon véhicule ?</a> </h4>
              </div>
              <div class="panel-collapse collapse" :class="[{'in' : choice === 'i'}]">
                <div class="panel-body">
                  <UL>Recopiez exactement les données de la carte grise (nom, prénom,immatriculation, numéro de formule) et votre date naissance</UL>
                  <UL>Seul les véhicules figurant dans le Sytème d'Immatriculation des Véhicules depuis 2009 peuvent être consultés dans Histovec</UL>
                  <UL> Il se peut aussi qu'il y ait une erreur sur la date de naissance enregistrée dans le système d’immatriculation des véhicules (SIV),</UL>
                  <UL><a :href="'mailto:histovec@interieur.gouv.fr?subject=Signaler%20une%20erreur'">contactez-nous</a></UL>
                </div>
              </div>
            </div>
            <!-- fin question 9 -->
            <!-- debut question 10 -->
            <div class="panel panel-default">
              <div class="panel-heading">
                <h4 class="panel-title"> <a @click="choose('j')" class="clickable" :class="[{'collapsed' : choice !== 'j' }]"> <i class="fa fa-file-text-o pr-10"></i>Je ne trouve pas le numéro de formule ?</a> </h4>
              </div>
              <div class="panel-collapse collapse" :class="[{'in' : choice === 'j'}]">
                <div class="panel-body">
                  <UL>Le numéro de formule est situé en bas à gauche de la carte grise. (p. ex. : 2015XX012345)</UL>
                </div>
              </div>
            </div>
            <!-- fin question 10 -->
            <!-- debut question 11 -->
            <div class="panel panel-default">
              <div class="panel-heading">
                <h4 class="panel-title"> <a @click="choose('k')" class="clickable" :class="[{'collapsed' : choicie !== 'k' }]"> <i class="fa fa-file-text-o pr-10"></i>Quelle est la politique de protection des données personnelles ?</a> </h4>
              </div>
              <div class="panel-collapse collapse" :class="[{'in' : choice === 'k'}]">
                <div class="panel-body">
                  <UL>Vous pouvez les consulter dans <a href="legal">mentions légales.</a></UL>
                </div>
              </div>
            </div>
            <!-- fin question 11 -->
          </div>
          <!-- accordion end -->
        </div>
      </div>
      <!-- row -->
    </div>
    <!-- container -->
  </div>
</template>

<script>
export default {
  data () {
    return {
      choice: ''
    }
  },
  methods: {
    choose (id) {
      console.log(this.choice, id)
      if (this.choice === id) {
        this.choice = ''
      } else {
        this.choice = id
      }
    }
  }
}
</script>
