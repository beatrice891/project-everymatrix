<template>
    <div class="container">
       <nav class="navbar navbar-expand-lg navbar-light bg-success">
            <a class="navbar-brand" href="#">
                <img src="../assets/logo.svg" height="40" alt="logo">
            </a>
            <button class="navbar-toggler custom-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
            </div>
        </nav>
    </div>
</template>
<script>
export default {
  
}
</script>

<style>
.form-control:focus {
    border-color: #28A745;
}
.custom-toggler .navbar-toggler-icon {
  background-image: url("data:image/svg+xml;charset=utf8,%3Csvg viewBox='0 0 32 32' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath stroke='rgba(255,255,255, 0.9)' stroke-width='2' stroke-linecap='round' stroke-miterlimit='10' d='M4 8h24M4 16h24M4 24h24'/%3E%3C/svg%3E");
}

.custom-toggler.navbar-toggler {
  border-color: rgb(255,255,255);
} 
.navbar-toggler:focus{
    outline: none;
}
.custom-toggler:hover{
    background-color: #1E5631;
}
</style>
