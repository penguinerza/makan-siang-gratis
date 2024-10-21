<script>
    import "../app.css";

    const pelantikan = new Date("2024-10-20T10:00:00.000+07:00")
    let currentTime = new Date()
    let TimeDiff = currentTime.getTime() - pelantikan.getTime()
    let diffDays = Math.floor(TimeDiff / (1000 * 3600 * 24))
</script>

<slot />

<div class="flex h-screen">
    <div class="m-auto">
        <h1 class="text-center">Makan Siang Gratis Counter</h1>
        <h2 class="text-center">{diffDays} Hari</h2>
    </div>
</div>
