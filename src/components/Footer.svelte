<script>
    import { wpLink, gitLink,instaLink, phoneNumber, locationLink, email, address } from '../config'
</script>
<style>


    .dark-green-bg {
        background: black;
    }
</style>

<section class="signup-section dark-green-bg" id="signup">
    <div class="container">
        <div class="row">
            <div class="col-md-10 mt-5 col-lg-8 mx-auto text-center">
                <i class="far fa-paper-plane fa-2x mb-2 text-white" />
                <h2 class="text-white mb-5">Inscreva-se para novidades!</h2>
                <form class="form-inline d-flex">
                    <input
                        class="form-control flex-fill mr-0 mr-sm-2 mb-3 mb-sm-0"
                        id="inputEmail"
                        name="EMAIL"
                        type="email"
                        placeholder="Digite o email..." />
                    <button
                    on:click={()=>alert("Desculpe, está funcionalidade ainda não foi ativada!")}
                        class="btn btn-primary mx-auto"
                        type="submit">Seguir</button>
                </form>
            </div>
        </div>
    </div>
</section>

<section class="contact-section dark-green-bg">
    <div class="container">
        <div class="row">
            <div class="col-md-6 mb-3 mb-md-0">
                <div class="card py-4 h-100">
                    <div class="card-body text-center">
                        <i class="fas fa-envelope text-primary mb-2" />
                        <h4 class="text-uppercase m-0">Email</h4>
                        <hr class="my-4" />
                        <div class="small text-black-50">
                            <p>{email}</p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="col-md-6 mb-3 mb-md-0">
                <div class="card py-4 h-100">
                    <div class="card-body text-center">
                        <i class="fas fa-mobile-alt text-primary mb-2" />
                        <h4 class="text-uppercase m-0">Telefone</h4>
                        <hr class="my-4" />
                        <div class="small text-black-50">
                            {phoneNumber}
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="social big d-flex justify-content-center">
            <a
                class="mx-2"
                target="_blank"
                href={wpLink}><i
                    class="fab fa-whatsapp" /></a>
            <a
                class="mx-2"
                target="_blank"
                href={gitLink}><i
                    class="fab fa-github" /></a>
        </div>
    </div>
</section>
<footer class="footer dark-green-bg big text-center text-white-50">
    <div class="container">Copyright © VinicPotifólio 2021</div>
</footer>
