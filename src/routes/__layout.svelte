<script>
    import "../app.css";
</script>

<header class="flex items-center sm:justify-center w-full max-w-5xl p-4">
    <img alt="Website Logo" src='/logo.svg' class="w-12 hidden sm:block"/>
    <h1 class="text-3xl sm:text-5xl font-display text-primary cursor-pointer">Sudden<span class="text-accent">Review</span></h1>
    <div  class="grow justify-end items-center">
        <nav class="flex grow justify-end items-center gap-4 ">
            <a href='/' class="py-1 px-2"><span class="nav-link">Home</span></a>
            <a href='/about' class="py-1 px-2"><span class="nav-link">About</span></a>
            <a href='/login' class="py-1 px-2 create-link">Start Now</a>
        </nav>
    </div>
</header>

<main class="flex flex-col grow w-full items-center mt-20 gap-5">
    <slot />
</main>

<footer class="text-sm my-4 text-neutral-700">
    SuddenReview is currently under development.
</footer>

<style>
    .nav-link {
        @apply font-semibold transition-all border-b border-neutral-200 hover:text-accent;
    }

    .create-link {
        @apply bg-primary text-light rounded font-semibold hover:text-accent transition-all;
    }
</style>