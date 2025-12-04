---
layout: page
title: Home
---

<main class="container" id="under-construction">
    <div class="glow" aria-hidden="true"></div>
    <div class="inner">
        <div class="icon-wrap" aria-hidden="true">
            <div class="icon-ring"></div>
            <div class="icon-inner">
                <!-- Simple cog SVG -->
                <svg class="cog" viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg">
                    <path fill="#38bdf8"
                        d="M36.9 6.2c-.6-2.2-3.2-3.2-5.2-2l-3.1 1.9c-1.3.8-2.9.5-3.9-.6l-1.4-1.6c-1.6-1.8-4.4-1.7-5.9.1l-4 4.7c-1.4 1.7-1.1 4.2.6 5.6l1.6 1.4c1.1.9 1.5 2.5.9 3.8l-1.5 3.3c-.4.9-1.2 1.6-2.1 1.9l-2.2.7c-2.2.7-3.5 3-2.8 5.2l1.8 5.7c.7 2.2 3 3.5 5.2 2.9l2.3-.7c1-.3 2 .1 2.7.8l2.5 2.6c.8.8 1.1 1.9.9 3l-.4 2.3c-.4 2.3 1.1 4.4 3.3 4.9l5.8 1.2c2.3.5 4.5-1 4.9-3.3l.4-2.3c.2-1.1.9-2.1 1.9-2.6l3.1-1.7c.9-.5 2-.5 2.9 0l2.1 1.2c2 1.1 4.6.3 5.6-1.9l2.5-5.4c1-2.2.1-4.8-2.1-5.8L53 35c-1-.4-1.7-1.3-2-2.3l-.9-3.4c-.3-1.2.1-2.4 1-3.2l2-1.9c1.7-1.6 1.8-4.4.2-6.1l-4-4.3c-1.6-1.7-4.2-1.7-5.9-.1L41 15c-.9.9-2.2 1.2-3.4.7l-2.6-1c-1-.5-1.7-1.4-1.9-2.5l.8-6z"
                        opacity="0.95" />
                    <circle cx="32" cy="32" r="11" fill="#020617" />
                    <circle cx="32" cy="32" r="6.5" fill="#e5f3ff" />
                </svg>
            </div>
        </div>
        <div class="pill">
            <span class="pill-dot"></span>
            <span>Work in progress</span>
        </div>
        <h1><span>This page is under construction</span></h1>
        <p>
            We’re busy assembling something new here. Check back soon to see the
            finished build.
        </p>
        <div class="progress" aria-hidden="true">
            <div class="progress-bar"></div>
        </div>
        <div class="footer">
            <span>It’ll be worth the wait. 🚧</span>
        </div>
    </div>
</main>

<style>
    :root {
        --bg: #050816;
        --accent: #38bdf8;
        --accent-soft: rgba(56, 189, 248, 0.2);
        --text-main: #f9fafb;
        --text-subtle: #9ca3af;
    }

    * {
        box-sizing: border-box;
        margin: 0;
        padding: 0;
    }

    body {
        min-height: 100vh;
        display: flex;
        align-items: center;
        justify-content: center;
        font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI",
            sans-serif;
        background: radial-gradient(circle at top, #111827 0, var(--bg) 55%);
        color: var(--text-main);
        overflow: hidden;
    }

    .container {
        position: relative;
        max-width: 480px;
        width: 90%;
        padding: 2.5rem 2rem 2.75rem;
        border-radius: 1.5rem;
        background: radial-gradient(circle at top left, #111827 0, #020617 60%);
        box-shadow:
            0 24px 60px rgba(15, 23, 42, 0.9),
            0 0 0 1px rgba(148, 163, 184, 0.15);
        border: 1px solid rgba(148, 163, 184, 0.2);
        backdrop-filter: blur(18px);
        opacity: 0;
        transform: translateY(10px) scale(0.98);
        transition:
            opacity 500ms ease-out,
            transform 500ms ease-out;
    }

    .container.visible {
        opacity: 1;
        transform: translateY(0) scale(1);
    }

    .glow {
        position: absolute;
        inset: -1px;
        border-radius: inherit;
        background: radial-gradient(circle at top,
                rgba(56, 189, 248, 0.18),
                transparent 60%);
        pointer-events: none;
        mix-blend-mode: screen;
        opacity: 0.7;
    }

    .inner {
        position: relative;
        z-index: 1;
    }

    .icon-wrap {
        width: 80px;
        height: 80px;
        border-radius: 999px;
        display: flex;
        align-items: center;
        justify-content: center;
        margin: 0 auto 1.75rem;
        background: radial-gradient(circle, #0f172a 0, #020617 65%);
        box-shadow:
            0 0 0 1px rgba(148, 163, 184, 0.25),
            0 18px 35px rgba(15, 23, 42, 0.8);
        position: relative;
        overflow: hidden;
    }

    .icon-ring {
        position: absolute;
        width: 140%;
        height: 140%;
        background: conic-gradient(from 0deg,
                rgba(56, 189, 248, 0.1),
                rgba(56, 189, 248, 0.6),
                rgba(56, 189, 248, 0.1));
        filter: blur(12px);
        opacity: 0.6;
        animation: spin 6s linear infinite;
    }

    .icon-inner {
        position: relative;
        z-index: 1;
        width: 52px;
        height: 52px;
    }

    .cog {
        width: 100%;
        height: 100%;
        animation: spin 4s linear infinite;
        filter: drop-shadow(0 4px 10px rgba(15, 23, 42, 0.9));
    }

    h1 {
        text-align: center;
        font-size: 1.6rem;
        letter-spacing: 0.04em;
        margin-bottom: 0.75rem;
    }

    h1 span {
        background: linear-gradient(120deg, #38bdf8, #a855f7);
        -webkit-background-clip: text;
        background-clip: text;
        color: transparent;
    }

    p {
        text-align: center;
        font-size: 0.98rem;
        color: var(--text-subtle);
        line-height: 1.6;
        margin-bottom: 1.75rem;
    }

    .pill {
        display: inline-flex;
        align-items: center;
        gap: 0.4rem;
        padding: 0.35rem 0.75rem;
        border-radius: 999px;
        font-size: 0.75rem;
        letter-spacing: 0.08em;
        text-transform: uppercase;
        background: rgba(15, 23, 42, 0.9);
        border: 1px solid rgba(148, 163, 184, 0.5);
        color: var(--text-subtle);
        margin: 0 auto 1.25rem;
    }

    .pill-dot {
        width: 8px;
        height: 8px;
        border-radius: 999px;
        background: var(--accent);
        box-shadow: 0 0 12px rgba(56, 189, 248, 0.9);
    }

    .progress {
        position: relative;
        width: 100%;
        height: 6px;
        border-radius: 999px;
        background: rgba(15, 23, 42, 0.9);
        overflow: hidden;
        box-shadow: inset 0 0 0 1px rgba(15, 23, 42, 0.9);
    }

    .progress-bar {
        position: absolute;
        inset: 0;
        background: linear-gradient(90deg, var(--accent-soft), var(--accent));
        transform-origin: left;
        animation: loading 2.8s ease-in-out infinite;
    }

    .footer {
        margin-top: 1rem;
        text-align: center;
        font-size: 0.75rem;
        color: #6b7280;
    }

    @keyframes spin {
        to {
            transform: rotate(360deg);
        }
    }

    @keyframes loading {
        0% {
            transform: scaleX(0.05);
        }

        40% {
            transform: scaleX(0.7);
        }

        70% {
            transform: scaleX(0.4);
        }

        100% {
            transform: scaleX(1);
        }
    }

    @media (max-width: 480px) {
        .container {
            padding: 2rem 1.5rem 2.25rem;
        }

        h1 {
            font-size: 1.4rem;
        }
    }
</style>
