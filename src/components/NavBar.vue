<template>
    <div id="nav">
        <nav class="navbar navbar-expand-lg navbar-light bg-secondary">
         <div class="container-fluid">
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                    <li class="nav-item">
                        <router-link to="/" class="nav-link active" aria-current="page">Home</router-link> 
                    </li> |
                    <li class="nav-item">
                       <router-link to="/about" class="nav-link active" aria-current="page">About</router-link>
                    </li> |
                    <li class="nav-item">
                        <router-link to="/contact" class="nav-link active" aria-current="page">Contact</router-link> 
                     </li> 
                </ul>
                <form class="d-flex">
                    <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
                    <button class="btn btn-outline-success" type="submit">Search</button>
                </form>
            </div>
         </div>
        </nav>
    </div>
</template>

