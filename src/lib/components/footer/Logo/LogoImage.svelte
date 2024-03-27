<script>
	export let imageUrl;
	export let altText;
</script>

<figure class="footer-logo__mask">
    <img class="footer-logo" src={imageUrl} alt={altText}>
</figure>

<style>
    .footer-logo__mask {
        width: 100px;
        height: 100px;
        border-radius: 50%;
        overflow: hidden;
        margin-bottom: 28px;
        box-shadow: 0 8px 16px rgba(0, 0, 0, 0.16);
    }

    .footer-logo {
        width: 100%;
        transform: scale(1.5);
        padding-top: 5px;
    }
</style>
