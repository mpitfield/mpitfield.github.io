---
layout: page
title: Home
---

<div class="construction-page">
    <div class="construction-modal">
        <img src="cog.png" width="100%">
        <h1>This is a development site</h1>
    </div>
</div>
<style>
    body {
        background: radial-gradient(circle at top, #111827 0, #050816 55%);
    }
    .construction-modal {
        max-width: 480px;
        width: 90%;
        background: radial-gradient(circle at top left, #111827 0, #020617 60%);
        box-shadow: 0 24px 60px rgba(15, 23, 42, 0.9), 0 0 0 1px rgba(148, 163, 184, 0.15);
        border: 1px solid rgba(148, 163, 184, 0.2);
        backdrop-filter: blur(18px);
        border-radius: 20px;
        color: white;
        text-align: center;
    }
    .construction-page {
        width: 100%;
        height: 100%;
        position: fixed;
        display: flex;
        align-items: center;
        justify-content: center;
    }
    .construction-modal img {
        width: 50%;
        margin: 50px auto 20px auto;
    }
    .construction-modal h1 {
        font-family: monospace;
        margin: 20px auto 50px auto;
    }
</style>
