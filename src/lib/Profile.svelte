<script>
    import me from '../assets/apple_brent.jpg'
    import Bio from './Bio.svelte'
    import Button from './Button.svelte'
    import Social from './Social.svelte'
</script>

<div class="font-mono antialiased text-gray-500 leading-normal tracking-wider ">
    <div
        class="max-w-4xl flex items-center h-auto lg:h-screen flex-wrap mx-auto my-32 lg:my-0"
    >
        <!--Main Col-->
        <div
            id="profile"
            class="w-full lg:w-1/2 rounded-lg lg:rounded-l-lg lg:rounded-r-none shadow-2xl bg-white  mx-6 lg:mx-0"
        >
            <div class="p-4 md:p-12 text-center lg:text-left">
                <!-- Image for mobile view-->
                <div
                    class="block lg:hidden rounded-full shadow-xl mx-auto -mt-16 h-48 w-48 bg-cover bg-top"
                    style="background-image: url('{me}')"
                />

                <Bio />

                <Button />

                <Social />
            </div>
        </div>

        <!--Img Col-->
        <div class="w-full lg:w-1/2">
            <!-- Big profile image for side bar (desktop) -->
            <img
                src={me}
                class="rounded-none lg:rounded-lg shadow-2xl hidden lg:block"
                alt="Brent Brinkley"
            />
            <!-- Image from: http://unsplash.com/photos/MP0IUfwrn0A -->
        </div>
    </div>
</div>
