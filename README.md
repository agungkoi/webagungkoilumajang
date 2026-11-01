# webagungkoilumajang
<script>
    tailwind.config = {
        theme: {
            extend: {
                colors: {
                    koi: {
                        dark: '#07090e',
                        card: 'rgba(15, 18, 28, 0.65)',
                        red: '#e63946',
                        orange: '#ff6b35',
                        gold: '#ffd166',
                        emerald: '#06d6a0',
                        accent: '#ff8c42'
                    }
                },
                fontFamily: {
                    serif: ['"Cormorant Garamond"', 'serif'],
                    sans: ['"Plus Jakarta Sans"', 'sans-serif']
                }
            }
        }
    }
</script>

<style>
    body {
        background-color: #07090e;
        color: #f1f5f9;
        font-family: 'Plus Jakarta Sans', sans-serif;
        overflow-x: hidden;
    }

    /* Abstract Koi Scale Dot Grid Pattern Overlay */
    .dot-grid-bg {
        background-image: radial-gradient(rgba(255, 107, 53, 0.15) 1.5px, transparent 1.5px);
        background-size: 24px 24px;
    }

    /* Glassmorphism Styling */
    .glass-card {
        background: rgba(15, 20, 32, 0.6);
        backdrop-filter: blur(16px);
        -webkit-backdrop-filter: blur(16px);
        border: 1px solid rgba(255, 107, 53, 0.2);
        box-shadow: 0 10px 30px -10px rgba(0, 0, 0, 0.7),
                    0 0 15px rgba(255, 107, 53, 0.05);
        transition: all 0.5s cubic-bezier(0.2, 0.8, 0.2, 1);
    }

    .glass-card:hover {
        border-color: rgba(255, 107, 53, 0.5);
        box-shadow: 0 20px 40px -15px rgba(255, 107, 53, 0.25),
                    0 0 25px rgba(230, 57, 70, 0.2);
        transform: translateY(-8px);
    }

    /* Ambient Liquid Ink Wash Orbs */
    .ink-wash-1 {
        position: fixed;
        top: -10%;
        left: -10%;
        width: 50vw;
        height: 50vw;
        background: radial-gradient(circle, rgba(230, 57, 70, 0.25) 0%, rgba(255, 107, 53, 0.08) 50%, transparent 70%);
        filter: blur(80px);
        pointer-events: none;
        z-index: 1;
        animation: floatGlow 18s ease-in-out infinite alternate;
    }

    .ink-wash-2 {
        position: fixed;
        bottom: -15%;
        right: -10%;
        width: 55vw;
        height: 55vw;
        background: radial-gradient(circle, rgba(255, 107, 53, 0.22) 0%, rgba(230, 57, 70, 0.05) 50%, transparent 70%);
        filter: blur(90px);
        pointer-events: none;
        z-index: 1;
        animation: floatGlow 22s ease-in-out infinite alternate-reverse;
    }

    @keyframes floatGlow {
        0% { transform: translate(0, 0) scale(1); }
        50% { transform: translate(40px, 30px) scale(1.1); }
        100% { transform: translate(-30px, 50px) scale(0.95); }
    }

    /* Custom Scrollbar */
    ::-webkit-scrollbar {
        width: 8px;
    }
    ::-webkit-scrollbar-track {
        background: #07090e;
    }
    ::-webkit-scrollbar-thumb {
        background: #2a1b18;
        border-radius: 4px;
        border: 1px solid rgba(255,107,53,0.2);
    }
    ::-webkit-scrollbar-thumb:hover {
        background: #ff6b35;
    }

    /* Water Ripple Effect */
    .ripple {
        position: absolute;
        border-radius: 50%;
        border: 1px solid rgba(255, 107, 53, 0.4);
        animation: ripple-anim 1.2s ease-out forwards;
        pointer-events: none;
    }
    @keyframes ripple-anim {
        0% { width: 0px; height: 0px; opacity: 1; transform: translate(-50%, -50%); }
        100% { width: 160px; height: 160px; opacity: 0; transform: translate(-50%, -50%); }
    }

    /* Text Gold Gradient */
    .text-gradient-gold {
        background: linear-gradient(135deg, #FFF 0%, #FFD1A9 50%, #FF6B35 100%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
    }
</style>
