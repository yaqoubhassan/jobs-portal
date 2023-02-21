<template>
    <header>
        <nav class="navbar navbar-expand-lg fixed-top" id="nav">
            <div class="container py-2">
                <a class="navbar-brand" href="#"><img src="../assets/logo.png" alt="" style="width: 50%;" class="logo"></a>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
                    data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false"
                    aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarSupportedContent">
                    <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
                        <li class="nav-item">
                            <a class="nav-link" aria-current="page" href="#">Home</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Jobs</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Blog</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">About Us</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Contact Us</a>
                        </li>
                    </ul>
                    <div class="ms-auto">
                        <a href="#" id="register-btn" class="hover-up me-5">Register</a>
                        <button class="signIn-btn">Sign In</button>
                    </div>
                </div>
            </div>
        </nav>
    </header>
</template>

<script>
    export default {
        
    }

    document.addEventListener('DOMContentLoaded', function () {
        window.addEventListener('scroll', myFunction);

        var navbar = document.getElementById("nav");
        var sticky = navbar.offsetTop;

        function myFunction() {
            if (window.pageYOffset > sticky) {
                navbar.classList.add("sticky")
            } else {
                navbar.classList.remove("sticky");
            }
        }
    });
</script>

<style scoped>
    .navbar {
        background-color: #FFFF;
        border-bottom: 1px solid #e8ecfa;
        box-shadow: 0px 20px 120px -30px gray;
        transition: all ease .65s;
    }

    .sticky {
        position: fixed;
        top: 0;
        padding: 0px;
        animation: 700ms ease-in-out 0s normal none 1 running fadeInDown;
    }
    .nav-item {
        margin: 0px 10px;
    }

    .nav-link {
        font-family: "Plus Jakarta Sans", sans-serif;
        font-style: normal;
        font-weight: 600;
        font-size: 14px;
        line-height: 18px;
        color: #05264E;
        display: block;
        text-decoration: none;
        position: relative;
    }

    .nav-link:hover {
        color: #3C65F5;
        border-bottom: 3px solid #3C65F5;
        padding-bottom: 1px;
    }

    #register-btn {
        font-family: "Plus Jakarta Sans", sans-serif;
        font-style: normal;
        font-weight: 500;
        font-size: 14px;
        line-height: 150%;
        color: #05264E;
        display: inline-block;
        position: relative;
        text-decoration-line: underline;
        position: relative;
        top: 0;
        transition: top ease 0.3s;
    }

    #register-btn:hover {
        top: -2px;
        color: #3C65F5;
    }

    .signIn-btn {
        color: #ffffff;
        background-color: #3C65F5;
        line-height: 26px;
        padding: 10px 20px;
        border-radius: 8px;
        font-size: 14px;
        border: 1px solid transparent;
        position: relative;
        top: 0;
        transition: top ease 0.3s;
    }

    .signIn-btn:hover {
        top: -2px;
        background-color: #05264E;
    }

    @keyframes fadeInDown {
        0% {opacity: 0; transform: translate3d(0,-100%,0);}
        100% {opacity: 1; -webkit-transform: translateZ(0);}
    }
</style>

