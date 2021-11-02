<template>
   <section class="contact" id="contact">
       <h2 class="get_in_touch h2">Get in Touch</h2>
        <div class="skills_header">
            <div class="line"></div>
        </div>
        <br><br>
        <form class="form" id="form">
            <div class="input_flex">
                <div class="name">
                    <input type="text" id="name" placeholder="Name">
                </div>
                    
                <div class="email">
                    <input type="email" id="email" placeholder="Email">
                </div>
                    
            </div>

            <div>
                <input type="text" id="message" placeholder="Message">
            </div>

            <button class="submit">Send Message</button>
                
        </form>
   </section>
</template>

<script>
export default {
    name: 'Contact'
}
</script>

<style>

</style>