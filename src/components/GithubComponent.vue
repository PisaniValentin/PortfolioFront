<template>
    <header>
        <ion-icon name="logo-github"></ion-icon>
        <p>Pisani Valentin</p>
        <div>
            <ion-icon name="search-circle-outline"></ion-icon>
        </div>
        <p style="color:#F78166">___________________</p>
    </header>
    <main>
        <div class="projectContainer">
            <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true"
                class="">
                <path
                    d="M2 2.5A2.5 2.5 0 0 1 4.5 0h8.75a.75.75 0 0 1 .75.75v12.5a.75.75 0 0 1-.75.75h-2.5a.75.75 0 0 1 0-1.5h1.75v-2h-8a1 1 0 0 0-.714 1.7.75.75 0 1 1-1.072 1.05A2.495 2.495 0 0 1 2 11.5Zm10.5-1h-8a1 1 0 0 0-1 1v6.708A2.486 2.486 0 0 1 4.5 9h8ZM5 12.25a.25.25 0 0 1 .25-.25h3.5a.25.25 0 0 1 .25.25v3.25a.25.25 0 0 1-.4.2l-1.45-1.087a.249.249 0 0 0-.3 0L5.4 15.7a.25.25 0 0 1-.4-.2Z">
                </path>
            </svg>
            <a href="">ProjectName</a>
            <p>Visibility</p>
            <p>:::</p>
            
        </div>
        <div class="projectContainer">
            <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true"
                class="">
                <path
                    d="M2 2.5A2.5 2.5 0 0 1 4.5 0h8.75a.75.75 0 0 1 .75.75v12.5a.75.75 0 0 1-.75.75h-2.5a.75.75 0 0 1 0-1.5h1.75v-2h-8a1 1 0 0 0-.714 1.7.75.75 0 1 1-1.072 1.05A2.495 2.495 0 0 1 2 11.5Zm10.5-1h-8a1 1 0 0 0-1 1v6.708A2.486 2.486 0 0 1 4.5 9h8ZM5 12.25a.25.25 0 0 1 .25-.25h3.5a.25.25 0 0 1 .25.25v3.25a.25.25 0 0 1-.4.2l-1.45-1.087a.249.249 0 0 0-.3 0L5.4 15.7a.25.25 0 0 1-.4-.2Z">
                </path>
            </svg>
            <a href="">ProjectName</a>
            <p>Visibility</p>
            <p>:::</p>
        </div>
        <div class="projectContainer">
            <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true"
                class="">
                <path
                    d="M2 2.5A2.5 2.5 0 0 1 4.5 0h8.75a.75.75 0 0 1 .75.75v12.5a.75.75 0 0 1-.75.75h-2.5a.75.75 0 0 1 0-1.5h1.75v-2h-8a1 1 0 0 0-.714 1.7.75.75 0 1 1-1.072 1.05A2.495 2.495 0 0 1 2 11.5Zm10.5-1h-8a1 1 0 0 0-1 1v6.708A2.486 2.486 0 0 1 4.5 9h8ZM5 12.25a.25.25 0 0 1 .25-.25h3.5a.25.25 0 0 1 .25.25v3.25a.25.25 0 0 1-.4.2l-1.45-1.087a.249.249 0 0 0-.3 0L5.4 15.7a.25.25 0 0 1-.4-.2Z">
                </path>
            </svg>
            <a href="">ProjectName</a>
            <p>Visibility</p>
            <p>:::</p>
        </div>
 

    </main>
</template>

<script>
export default {
    data() {
    },
    methods: {

    },
}
</script>



<style scoped>

header {
    display: flex;
    background: black;
    padding: 10px;
    color: white;
}

main {
    display: flex;
    flex-direction: column;
    align-items: center;
    background: #161b22;
    border-bottom-left-radius: 15px;
    gap: 10px;
    padding: 10px;
}

.projectContainer {
    border: 1px solid #30363d;
    border-radius: 5px;
    display: flex;
    gap: 10px;
    width: 80%;
}

</style>

<!-- https://api.github.com/users/PisaniValentin/repos -->