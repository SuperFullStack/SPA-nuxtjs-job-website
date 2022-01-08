<template>
<div class="container flex flex-col h-screen overflow-hidden">
    <Nav />
    <main class=" flex-1 overflow-y-scroll">
        <div class=" first-part ">
                <Agreement />
        </div>
        <Sections />
    </main>
    <Footer />
</div>
</template>

<script>
export default {

}
</script>

<style>
 @import url('https://fonts.googleapis.com/css2?family=Lato:wght@400;700&display=swap');
.first-part{
    font-family: 'Lato', sans-serif;
    background: transparent linear-gradient(141deg, #EBF4FF 0%, #E6FFFA 100%) 0% 0% no-repeat padding-box;
    opacity: 1; 
}

.container{
    background: #FFFFFF 0% 0% no-repeat padding-box;
    opacity: 1;
}

</style>