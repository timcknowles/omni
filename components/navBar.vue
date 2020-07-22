<template>
    <b-navbar>
        <template slot="brand">
            <b-navbar-item tag="router-link" :to="{ path: '/' }">
            
                <img
                        src="~/static/ACCU_banner.png"
                        alt="RLH logo"
                    >
           
            </b-navbar-item>
        
        </template>
        <template slot="start">
            <b-navbar-item href="/">
                Home
            </b-navbar-item>
            <b-navbar-item href="/">
                Re-circulation
            </b-navbar-item>
            <b-navbar-item href="/">
                Access
            </b-navbar-item>
            <b-navbar-item href="/">
                Hyperkalaemia
            </b-navbar-item>
            <b-navbar-dropdown label="Anticoagulation">
                <b-navbar-item href="#">
                    systemic anticoagulation
                </b-navbar-item>
                <b-navbar-item href="#">
                    VTE
                </b-navbar-item>
            </b-navbar-dropdown>
        </template>

        <!-- <template slot="end">
            <b-navbar-item tag="div">
                <div class="buttons">
                    <a class="button is-primary">
                        <strong>Sign up</strong>
                    </a>
                    <a class="button is-light">
                        Log in
                    </a>
                </div>
            </b-navbar-item>
        </template> -->
    </b-navbar>
</template>