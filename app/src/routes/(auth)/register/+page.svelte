<script>
	import Small from "../../../components/Texts/Small.svelte";


	import Title from "../../../components/Texts/Title.svelte";
    import IconMail from '~icons/fa-solid/envelope'; 
    import IconLock from '~icons/mdi/lock';
</script>


<section>
        <div>
            <Title text = "Hi" />
            <Title text = "Welcome back" />
            <Small text = "Fill out all the fields" />
            <form class="flex flex-col items-center gap-5 mt-5">
                <div class="flex items-center gap-2 border-r-10 border-seaBlue w-80 h-13 bg-lowWhite px-3 @md:w-100 @md:h-15 @xl:w-80 @2xl:w-100 @2xl:h-15 @4xl:w-120">
                    <IconMail class="text-seaBlue text-2xl" />
                    <input type="email" placeholder="Email" class="outline-none border-none bg-transparent flex-1 h-full text-lg">
                </div>
                <div class="flex items-center gap-2 border-r-10 border-seaBlue w-80 h-13 bg-lowWhite px-3 @md:w-100 @md:h-15 @xl:w-80 @2xl:w-100 @2xl:h-15 @4xl:w-120">
                    <IconLock class="text-seaBlue text-2xl" />
                    <input type="password" placeholder="Password" class="outline-none border-none bg-transparent flex-1 h-full text-lg">
                </div>
                <div class="flex gap-10 justify-between w-full">
                    <Small text = "Forgot password?" />
                    <a href="/login" class="text-seaBlue">Login</a>
                </div>
                <button class="w-80 h-13 text-white font-bold bg-seaBlue rounded-md @md:w-100 @xl:w-80 @2xl:w-100 @4xl:w-120"><a href="/login">Register</a></button>
            </form>
        </div>
</section>