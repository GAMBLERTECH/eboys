
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MASTERS CYBER | Windows Installation & Perfume Refill</title>

<style>
:root {
  --navy: #16233b;
  --blue: #3156a6;
  --gold: #d7ad62;
  --light: #fff7ec;
  --surface: #ffffff;
  --surface-border: #eee5d8;
  --page-blue: linear-gradient(135deg, #fffaf2, #f7f1e8);
  --text: #29364b;
  --muted: #657187;
  --content-width: 72rem;
}

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  border: 0;
}

html {
  scroll-behavior: smooth;
  scroll-padding-top: 5.3125rem;
}

body {
  font-family: "Segoe UI", Arial, sans-serif;
  color: var(--text);
  line-height: 1.7;
  background: #fffaf4;
  overflow-x: hidden;
}

a {
  text-decoration: none;
  color: inherit;
}

.skip-link {
  position: fixed;
  top: 0.75rem;
  left: 0.75rem;
  z-index: 999;
  transform: translateY(-150%);
  border-radius: 0.5rem;
  background: var(--navy);
  color: #ffffff;
  padding: 0.625rem 0.875rem;
  font-size: 0.8125rem;
  font-weight: 700;
  transition: transform 0.2s ease;
}

.skip-link:focus {
  transform: translateY(0);
}

header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  min-height: 4.875rem;
  padding: 0.875rem max(6%, calc((100% - var(--content-width)) / 2));
  background: rgba(255, 255, 255, 0.94);
  backdrop-filter: blur(0.75rem);
  -webkit-backdrop-filter: blur(0.75rem);
  position: sticky;
  top: 0;
  z-index: 100;
  box-shadow: 0 0.375rem 1.5rem rgba(22, 35, 59, 0.06);
  border-bottom: 0.0625rem solid rgba(22, 35, 59, 0.08);
  transition: box-shadow 0.2s ease, background 0.2s ease;
}

header.scrolled {
  background: rgba(255, 255, 255, 0.98);
  box-shadow: 0 0.625rem 2rem rgba(22, 35, 59, 0.12);
}

a {
  color: inherit;
}

.logo {
  color: var(--navy);
  font-size: 1.25rem;
  font-weight: 900;
  line-height: 1.2;
}

.logo span {
  color: var(--blue);
}

.logo small {
  display: block;
  font-size: 0.625rem;
  letter-spacing: 0.125rem;
  margin-top: 0.3125rem;
}

nav {
  display: flex;
  align-items: center;
  gap: 1.5625rem;
}

nav a {
  font-size: 0.75rem;
  font-weight: 650;
  color: var(--text);
  padding: 0.625rem 0.125rem;
  transition: color 0.2s ease, border-color 0.2s ease;
  border-bottom: 0.125rem solid transparent;
}

nav a:hover {
  color: var(--blue);
  border-bottom-color: var(--blue);
}

nav a.active {
  color: var(--blue);
  border-bottom-color: var(--blue);
}

.menu-toggle {
  display: none;
  border: 0;
  background: none;
  font-size: 1.5625rem;
  cursor: pointer;
  color: var(--navy);
}

.hero {
  min-height: 35rem;
  display: grid;
  grid-template-columns: 1fr 1fr;
  align-items: center;
  gap: 3rem;
  padding: 5rem max(7%, calc((100% - var(--content-width)) / 2));
  background:
    radial-gradient(circle at 82% 18%, rgba(215, 173, 98, 0.16), transparent 18rem),
    var(--page-blue);
}

.tagline {
  color: var(--blue);
  font-size: 0.625rem;
  font-weight: bold;
  letter-spacing: 0.14rem;
  margin-bottom: 0.9375rem;
}

.hero h1 {
  color: var(--navy);
  font-size: clamp(2.75rem, 5vw, 4.25rem);
  line-height: 1.08;
  letter-spacing: -0.15rem;
  margin-bottom: 1.25rem;
}

.hero h1 span,
.perfume-content h2 span {
  color: var(--blue);
}

.hero-content > p:not(.tagline) {
  max-width: 30rem;
  color: var(--muted);
  font-size: 0.9375rem;
  margin-bottom: 1.75rem;
}

.hero-buttons {
  display: flex;
  gap: 0.75rem;
  flex-wrap: wrap;
}

.btn {
  display: inline-block;
  border: 0;
  border-radius: 999px;
  padding: 0.8125rem 1.25rem;
  background: var(--navy);
  color: white;
  font-size: 0.75rem;
  font-weight: bold;
  cursor: pointer;
  transition: transform 0.2s ease, background 0.2s ease, box-shadow 0.2s ease;
  box-shadow: 0 0.5rem 1.125rem rgba(22, 35, 59, 0.15);
}

.btn:hover {
  transform: translateY(-0.125rem);
  background: #263a5f;
  box-shadow: 0 0.75rem 1.5rem rgba(22, 35, 59, 0.2);
}

.btn-outline {
  background: #ffffff;
  border: 0.0625rem solid var(--surface-border);
  color: var(--navy);
  box-shadow: none;
}

.hero-image {
  display: grid;
  place-items: center;
}

.image-card {
  width: min(100%, 27.5rem);
  min-height: 22rem;
  padding: 2rem 1.5rem;
  border-radius: 1.5rem;
  text-align: center;
  background: #ffffff;
  box-shadow: 0 1.5rem 3.75rem rgba(22, 35, 59, 0.12);
  border: 0.0625rem solid rgba(22, 35, 59, 0.06);
}

.hero-visuals {
  min-height: 13.75rem;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 1.25rem;
  margin-bottom: 1rem;
  border-radius: 1.125rem;
  background: linear-gradient(135deg, #f2f5fa, #fbf8f0);
}

.laptop {
  font-size: 6rem;
  filter: drop-shadow(0 0.75rem 1.125rem rgba(68, 115, 255, 0.18));
}

.perfume-bottle {
  position: relative;
  width: 6rem;
  height: 8.75rem;
  margin: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  filter: drop-shadow(0 1rem 1.5rem rgba(214, 160, 66, 0.28));
}

.perfume-cap {
  position: absolute;
  top: -1.125rem;
  width: 2.625rem;
  height: 1.5rem;
  border-radius: 0.5rem 0.5rem 0.25rem 0.25rem;
  background: linear-gradient(180deg, #f7df9a, #c78d32);
  box-shadow: inset 0 0.125rem 0.375rem rgba(255,255,255,0.8);
}

.perfume-cap::before {
  content: "";
  position: absolute;
  inset: 0.25rem 0.4375rem 0.375rem;
  border-radius: 0.25rem;
  background: linear-gradient(180deg, rgba(255,255,255,0.9), rgba(255,255,255,0.15));
}

.perfume-glass {
  position: absolute;
  bottom: 0;
  width: 6rem;
  height: 7.875rem;
  border-radius: 1.125rem 1.125rem 1.625rem 1.625rem;
  background: linear-gradient(180deg,
    rgba(255, 255, 255, 0.95) 0%,
    rgba(255, 239, 202, 0.88) 12%,
    rgba(215, 173, 87, 0.82) 42%,
    rgba(145, 95, 36, 0.86) 100%
  );
  border: 0.125rem solid rgba(255,255,255,0.9);
  box-shadow: inset 0 0 0.75rem rgba(255,255,255,0.8), inset 0.75rem 0 1.125rem rgba(255,255,255,0.45), inset -0.75rem 0 1.125rem rgba(109, 68, 16, 0.18);
  overflow: hidden;
}

.perfume-glass::before {
  content: "";
  position: absolute;
  inset: 0;
  background: linear-gradient(120deg, rgba(255,255,255,0.65) 0%, rgba(255,255,255,0.08) 28%, transparent 50%, rgba(255,255,255,0.2) 100%);
  transform: skewX(-18deg);
}

.perfume-glass::after {
  content: "";
  position: absolute;
  inset: 0.875rem 1.5rem 1.125rem 1.5rem;
  border-radius: 0.75rem;
  border: 0.0625rem solid rgba(255,255,255,0.75);
  background: rgba(255,255,255,0.12);
}

.image-card h3 {
  margin-top: 0.625rem;
  color: var(--navy);
}

.image-card p {
  color: var(--muted);
  font-size: 0.8125rem;
}

.section {
  padding: 5rem max(7%, calc((100% - var(--content-width)) / 2));
  scroll-margin-top: 4.875rem;
}

.section-heading {
  text-align: center;
  margin: 0 auto 2.5rem;
  max-width: 42rem;
}

.section-heading h2 {
  font-size: clamp(1.8125rem, 4vw, 2.5rem);
  color: var(--navy);
  line-height: 1.2;
  letter-spacing: -0.04rem;
}

.section-heading > p:last-child {
  color: var(--muted);
  font-size: 0.8125rem;
  margin-top: 0.75rem;
}

.cards {
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  gap: 1rem;
}

.card {
  position: relative;
  padding: 1.5rem 1.25rem;
  border: 0.0625rem solid var(--surface-border);
  border-radius: 0.875rem;
  transition: transform 0.2s ease, box-shadow 0.2s ease, border-color 0.2s ease;
  background: var(--surface);
  box-shadow: 0 0.5rem 1.5rem rgba(22, 35, 59, 0.04);
}

.card:hover {
  transform: translateY(-0.25rem);
  box-shadow: 0 1rem 2rem rgba(22, 35, 59, 0.09);
  border-color: #c6d1e1;
}

.card::after {
  content: "";
  position: absolute;
  left: 1.25rem;
  right: 1.25rem;
  bottom: 0;
  height: 0.1875rem;
  border-radius: 999px 999px 0 0;
  background: linear-gradient(90deg, var(--blue), var(--gold));
  transform: scaleX(0);
  transform-origin: left;
  transition: transform 0.25s ease;
}

.card:hover::after {
  transform: scaleX(1);
}

.card-icon {
  width: 3.3125rem;
  height: 3.3125rem;
  display: grid;
  place-items: center;
  border-radius: 0.875rem;
  background: #edf2fa;
  color: var(--blue);
  box-shadow: none;
  font-size: 1.5625rem;
  margin-bottom: 1.125rem;
}

.card h3 {
  font-size: 1rem;
  color: var(--navy);
  margin-bottom: 0.625rem;
}

.card p {
  font-size: 0.75rem;
  color: var(--muted);
  margin-bottom: 1.25rem;
}

.service-link {
  color: var(--blue);
  font-weight: bold;
  font-size: 0.6875rem;
}

.windows-section {
  padding-top: 0;
}

.windows-section .card {
  max-width: 34rem;
  margin: 0 auto;
}

.refill-section {
  padding: 5rem max(7%, calc((100% - var(--content-width)) / 2));
  background: #fff4e7;
}

.refill-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 1.375rem;
}

.refill-card {
  position: relative;
  padding: 1.5rem 1.25rem 1.25rem;
  background: #ffffff;
  border: 0.0625rem solid var(--surface-border);
  border-radius: 0.875rem;
  box-shadow: 0 0.625rem 1.5rem rgba(22, 35, 59, 0.05);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.refill-card:hover {
  transform: translateY(-0.25rem);
  box-shadow: 0 1rem 2rem rgba(22, 35, 59, 0.1);
}

.refill-badge {
  display: inline-block;
  padding: 0.375rem 0.625rem;
  border-radius: 999px;
  background: rgba(30, 64, 175, 0.12);
  color: var(--blue);
  font-size: 0.5625rem;
  font-weight: 700;
  letter-spacing: 0.09375rem;
  text-transform: uppercase;
  margin-bottom: 0.875rem;
}

.refill-card h3 {
  font-size: 1.125rem;
  color: var(--navy);
  margin-bottom: 0.625rem;
}

.refill-card p {
  color: var(--muted);
  font-size: 0.75rem;
  margin-bottom: 0.875rem;
}

.refill-card ul {
  list-style: none;
  margin: 0 0 1rem;
  display: grid;
  gap: 0.375rem;
}

.refill-card li {
  color: var(--text);
  font-size: 0.6875rem;
  position: relative;
  padding-left: 1rem;
}

.refill-card li::before {
  content: "•";
  position: absolute;
  left: 0;
  color: var(--gold);
  font-size: 1rem;
}

.refill-price {
  display: flex;
  align-items: baseline;
  justify-content: space-between;
  gap: 0.5rem;
  padding-top: 0.875rem;
  border-top: 0.0625rem solid rgba(148, 163, 184, 0.28);
  color: var(--navy);
  font-weight: 700;
}

.refill-price span {
  font-size: 0.625rem;
  color: var(--muted);
  font-weight: 600;
}

.perfume-section {
  background:
    radial-gradient(circle at 80% 48%, #354e78 0, transparent 36%),
    linear-gradient(125deg, #16233b, #263d65 65%, #354e78);
  color: white;
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 2.5rem;
  align-items: center;
  padding: 5rem max(8%, calc((100% - var(--content-width)) / 2));
}

.perfume-content h2 {
  font-size: clamp(2.375rem, 5vw, 3.4375rem);
  line-height: 1.15;
  margin-bottom: 1.25rem;
}

.perfume-content h2 span {
  color: var(--gold);
}

.perfume-content > p:not(.tagline) {
  color: #bdc7de;
  font-size: 0.8125rem;
}

.fragrance-options {
  display: grid;
  gap: 1.0625rem;
  margin: 1.875rem 0;
}

.fragrance-options > div {
  display: flex;
  align-items: center;
  gap: 0.9375rem;
}

.fragrance-options > div > span {
  width: 2.375rem;
  height: 2.375rem;
  display: grid;
  place-items: center;
  border: 0.0625rem solid #ffffff30;
  border-radius: 0.625rem;
  color: var(--gold);
  font-size: 1.25rem;
}

.fragrance-options h3 {
  font-size: 0.8125rem;
}

.fragrance-options p {
  color: #bdc7de;
  font-size: 0.6875rem;
}

.perfume-content .btn {
  background: linear-gradient(135deg, #ffdc86, #e9b84c);
  color: var(--navy);
  box-shadow: 0 0.5rem 1.375rem #f0c66b30;
}

.bottle-display {
  min-height: 23.25rem;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 1rem;
  position: relative;
  padding-bottom: 3rem;
}

.bottle {
  height: 9.6875rem;
  width: 5rem;
  border-radius: 0.75rem 0.75rem 1.125rem 1.125rem;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  font-size: 0.625rem;
  font-weight: bold;
  letter-spacing: 0.0625rem;
  color: #593f20;
  background: linear-gradient(100deg, #ae8146, #f0d9a5, #a47b41);
  border: 0.0625rem solid #dfc18b;
  box-shadow: inset 0.3125rem 0 0.75rem #ffffff50,
              0 1.25rem 1.5625rem #00000030;
  position: relative;
}

.bottle::before {
  content: "";
  position: absolute;
  width: 1.75rem;
  height: 1.6875rem;
  background: linear-gradient(90deg, #8e6c3c, #f2d7a0, #8e6c3c);
  top: -1.6875rem;
  border-radius: 0.25rem 0.25rem 0 0;
}

.bottle-one {
  transform: rotate(-8deg) scale(.85);
}

.bottle-two {
  height: 11.25rem;
  background: linear-gradient(100deg, #aebbd0, #f8fbff, #9ba9c0);
  z-index: 2;
}

.bottle-two::before {
  background: linear-gradient(90deg, #9da9ba, white, #9da9ba);
}

.bottle-three {
  transform: rotate(8deg) scale(.9);
  background: linear-gradient(100deg, #12244b, #365a9e, #12244b);
  color: #f3d58f;
}

.bottle-display > p {
  position: absolute;
  bottom: 0.3125rem;
  color: #b9c3dc;
  font-size: 0.5625rem;
  letter-spacing: 0.1875rem;
}

.why-us {
  background: var(--page-blue);
}

.benefits {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1.5625rem;
  margin-top: 2.1875rem;
  text-align: center;
}

.benefits > div {
  padding: 1.5625rem 0.9375rem;
  background: white;
  border: 0.0625rem solid var(--surface-border);
  border-radius: 0.875rem;
  box-shadow: 0 0.5rem 1.5rem rgba(22, 35, 59, 0.04);
}

.benefits span {
  display: inline-grid;
  place-items: center;
  width: 2.5rem;
  height: 2.5rem;
  background: #e4f7ed;
  color: #248b61;
  border-radius: 50%;
  font-size: 1.3125rem;
}

.benefits h3 {
  font-size: 0.9375rem;
  margin: 0.8125rem 0 0.4375rem;
}

.benefits p {
  color: var(--muted);
  font-size: 0.75rem;
}

.contact-section {
  padding: 5rem max(8%, calc((100% - var(--content-width)) / 2));
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 3.4375rem;
  background:
    radial-gradient(circle at 10% 10%, #354e78 0, transparent 36%),
    linear-gradient(125deg, #16233b, #263d65 65%, #354e78);
  color: white;
}

.contact-info h2 {
  font-size: clamp(1.875rem, 4vw, 2.625rem);
  line-height: 1.2;
  margin-bottom: 1.25rem;
}

.contact-info > p:not(.tagline) {
  color: #c4cee4;
  font-size: 0.8125rem;
  margin: 1.0625rem 0;
}

.contact-info small {
  display: block;
  margin-top: 1.875rem;
  color: #a9b6d3;
  font-size: 0.6875rem;
}

.contact-info p:not(.tagline) {
  display: flex;
  align-items: flex-start;
  gap: 0.625rem;
}

.contact-info p:not(.tagline)::before {
  color: var(--gold);
  width: 1.25rem;
  flex: 0 0 1.25rem;
  text-align: center;
}

.contact-info p:nth-of-type(3)::before {
  content: "●";
  font-size: 0.5rem;
  margin-top: 0.375rem;
}

.contact-info p:nth-of-type(4)::before {
  content: "☎";
}

.contact-info p:nth-of-type(5)::before {
  content: "◷";
}

.contact-form {
  background: #ffffff;
  color: var(--text);
  padding: 1.75rem;
  border-radius: 0.875rem;
  box-shadow: 0 1.25rem 3.4375rem rgba(8, 15, 40, 0.15);
  border: 0.0625rem solid rgba(255, 255, 255, 0.8);
}

.contact-form h3 {
  font-size: 1.3125rem;
  margin-bottom: 1.25rem;
  color: var(--navy);
}

.contact-form label {
  display: block;
  font-size: 0.75rem;
  font-weight: bold;
  margin: 0.875rem 0 0.375rem;
}

.contact-form input,
.contact-form select,
.contact-form textarea {
  width: 100%;
  padding: 0.75rem;
  border: 0.0625rem solid var(--surface-border);
  border-radius: 0.5rem;
  background: #fffaf4;
  font: inherit;
  font-size: 0.75rem;
  outline: none;
}

.contact-form input:focus,
.contact-form select:focus,
.contact-form textarea:focus {
  border-color: var(--blue);
  box-shadow: 0 0 0 0.1875rem #315cf515;
}

.contact-form textarea {
  resize: vertical;
}

.contact-form button {
  width: 100%;
  margin-top: 1.125rem;
}

#formMessage {
  font-size: 0.75rem;
  color: #b43d3d;
  margin-top: 0.625rem;
}

#formMessage.success {
  color: #248b61;
}

footer {
  text-align: center;
  padding: 1.875rem 0.9375rem;
  background: #111c30;
  color: #aeb9d1;
  font-size: 0.6875rem;
}

.footer-logo {
  display: inline-block;
  font-weight: 900;
  font-size: 1.125rem;
  color: rgba(255, 255, 255, 0.753);
  margin-bottom: 0.5rem;
}

footer p {
  margin-top: 0.3125rem;
}

.whatsapp-float {
  position: fixed;
  right: 1.25rem;
  bottom: 1.25rem;
  z-index: 90;
  width: 3.375rem;
  height: 3.375rem;
  display: grid;
  place-items: center;
  align-items: center;
  border-radius: 50%;
  background: #25d366;
  color: white;
  font-size: 1.5rem;
  font-weight: 800;
  box-shadow: 0 0.75rem 2rem rgba(4, 240, 90, 0.32);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.whatsapp-float:hover {
  transform: translateY(-0.1875rem);
  box-shadow: 0 1rem 2.5rem rgba(37, 211, 102, 0.38);
}

@media (max-width: 56.25rem) {
  .cards {
    grid-template-columns: repeat(2, 1fr);
  }

  .refill-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }

  .hero {
    padding-inline: 6%;
  }

  .contact-section {
    gap: 1.875rem;
    padding-inline: 6%;
  }
}

@media (max-width: 40.625rem) {
  header {
    min-height: 4.625rem;
    padding: 0.75rem 5%;
  }

  .menu-toggle {
    display: block;
  }

  nav {
    display: none;
    position: absolute;
    top: 100%;
    left: 0;
    right: 0;
    flex-direction: column;
    align-items: stretch;
    gap: 0;
    background: white;
    padding: 0.625rem 6% 1.25rem;
    box-shadow: 0 0.75rem 1.25rem #101c3b14;
  }

  nav.open {
    display: flex;
  }

  nav a {
    padding: 0.75rem 0;
    border-bottom: 0.0625rem solid #edf0f5;
  }

  .hero,
  .perfume-section,
  .contact-section {
    grid-template-columns: 1fr;
  }

  .hero {
    padding: 3.5rem 6%;
    gap: 1.875rem;
  }

  .hero h1 {
    font-size: 2.625rem;
  }

  .image-card {
    min-height: 19rem;
    padding: 1.5rem;
  }

  .hero-visuals {
    min-height: 12rem;
  }

  .laptop {
    font-size: 5rem;
  }

  .perfume-bottle {
    transform: scale(0.85);
  }

  .perfume-emoji {
    font-size: 3.75rem;
  }

  .section {
    padding: 3.75rem 6%;
  }

  .cards {
    grid-template-columns: 1fr;
  }

  .windows-section {
    padding-top: 0;
  }

  .refill-section {
    padding: 3.75rem 6%;
  }

  .refill-grid {
    grid-template-columns: 1fr;
  }

  .perfume-section {
    padding: 3.75rem 6%;
    gap: 2.1875rem;
  }

  .bottle-display {
    min-height: 17.5rem;
    gap: 0.5rem;
  }

  .bottle {
    width: 4.0625rem;
  }

  .benefits {
    grid-template-columns: 1fr;
    gap: 0.8125rem;
  }

  .contact-section {
    padding: 3.75rem 6%;
  }

  .contact-form {
    padding: 1.375rem 1.0625rem;
  }
}

@media (prefers-reduced-motion: reduce) {
  html {
    scroll-behavior: auto;
  }

  *, *::before, *::after {
    transition: none !important;
  }
}

:focus-visible {
  outline: 0.1875rem solid #d7ad62;
  outline-offset: 0.1875rem;
}
</style>
</head>

<body>

<a class="skip-link" href="#main-content">Skip to main content</a>

<header>
  <a href="#home" class="logo">
    MASTERS <span>CYBER</span>
    <small>CYBER • WINDOWS • FRAGRANCE</small>
  </a>

  <button class="menu-toggle" id="menuToggle"
          aria-label="Toggle navigation"
          aria-controls="navigation"
          aria-expanded="false">☰</button>

  <nav id="navigation" aria-label="Main navigation">
    <a href="#home">Home</a>
    <a href="#services">Cyber Services</a>
    <a href="#perfumes">Perfume Refill</a>
    <a href="#windows">Windows Installation</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<main id="main-content">
<section class="hero" id="home">
  <div class="hero-content">
    <p class="tagline">YOUR LOCAL SERVICE CENTRE</p>
    <h1>Digital Services.<br><span>Signature Scents.</span></h1>
    <p>
      Friendly support for everyday cyber needs, Windows installation
      and quality perfume refills—all in one convenient place.
    </p>

    <div class="hero-buttons">
      <a href="#services" class="btn">Explore Services</a>
      <a href="#contact" class="btn btn-outline">Contact Us</a>
    </div>
  </div>

  <div class="hero-image">
    <div class="image-card">
      <div class="hero-visuals" aria-hidden="true">
        <div class="laptop">💻</div>
        <div class="perfume-bottle">
          <div class="perfume-cap"></div>
          <div class="perfume-glass"></div>
        </div>
      </div>
      <h3>MASTERS Cyber & Perfume</h3>
      <p>Dependable service, with a personal touch.</p>
    </div>
  </div>
</section>

<section class="section" id="services">
  <div class="section-heading">
    <p class="tagline">WHAT WE OFFER</p>
    <h2>Our Cyber Services</h2>
    <p>Reliable assistance for your everyday digital needs.</p>
  </div>

  <div class="cards">
    <article class="card">
      <div class="card-icon">🖨️</div>
      <h3>Printing & Photocopying</h3>
      <p>Black-and-white and colour printing, photocopies and document editing.</p>
      <a href="#contact" class="service-link"
         data-service="Printing and photocopying">Enquire now →</a>
    </article>

    <article class="card">
      <div class="card-icon">🌐</div>
      <h3>Online Services</h3>
      <p>Assistance with online forms, digital submissions and other online services.</p>
      <a href="#contact" class="service-link"
         data-service="Online services">Enquire now →</a>
    </article>

    <article class="card">
      <div class="card-icon">📝</div>
      <h3>Typing & Scanning</h3>
      <p>Typing, scanning, CV formatting, proposal editing and bulk printing.</p>
      <a href="#contact" class="service-link"
         data-service="Typing and scanning">Enquire now →</a>
    </article>

    <article class="card">
      <div class="card-icon">🎨</div>
      <h3>Design & Binding</h3>
      <p>Posters, business designs, document binding and lamination.</p>
      <a href="#contact" class="service-link"
         data-service="Design and binding">Enquire now →</a>
    </article>
  </div>
</section>

<section class="section windows-section" id="windows">
  <div class="section-heading">
    <p class="tagline">WINDOWS INSTALLATION</p>
    <h2>Windows Installation & Setup</h2>
    <p>Reliable Windows installation and setup assistance for your computer.</p>
  </div>

  <article class="card">
    <div class="card-icon" aria-hidden="true">💻</div>
    <h3>Get Your Computer Ready</h3>
    <p>Get help installing Windows and setting up your computer. Contact us to set your  device .</p>
    <a href="#contact" class="service-link"
       data-service="Windows installation">Enquire now →</a>
  </article>
</section>

<section class="perfume-section" id="perfumes">
  <div class="perfume-content">
    <p class="tagline" style="color:var(--gold)">
      DISCOVER YOUR SIGNATURE SCENT
    </p>
    <h2>Fragrance That<br><span>Defines You.</span></h2>
    <p>
      Explore fragrance refills for different moods, personalities
      and occasions. Ask about available scents and bottle sizes.
    </p>

    <div class="fragrance-options">
      <div>
        <span>✦</span>
        <div>
          <h3>For Men</h3>
          <p>Fresh, woody and bold scents.</p>
        </div>
      </div>

      <div>
        <span>✧</span>
        <div>
          <h3>For Women</h3>
          <p>Floral, warm and elegant scents.</p>
        </div>
      </div>

      <div>
        <span>◇</span>
        <div>
          <h3>Unisex</h3>
          <p>Versatile scents for everyone.</p>
        </div>
      </div>
    </div>

    <a href="#contact" class="btn" data-service="Perfume refill">
      Enquire About Perfumes
    </a>
  </div>

  <div class="bottle-display">
    <div class="bottle bottle-one"><span>NO. 01<br>AMBER</span></div>
    <div class="bottle bottle-two"><span>NO. 02<br>PURE</span></div>
    <div class="bottle bottle-three"><span>NO. 03<br>OUD</span></div>
    <p>THE FRAGRANCE COLLECTION</p>
  </div>
</section>

<section class="refill-section">
  <div class="section-heading">
    <p class="tagline">PERFUME REFILL</p>
    <h2>Fresh Fragrance, Better Value</h2>
    <p>Choose a refill style that matches your scent and your routine.</p>
  </div>

  <div class="refill-grid">
    <article class="refill-card">
      <span class="refill-badge">Classic</span>
      <h3>Luxury Daily Refill</h3>
      <p>Clean, long-lasting scents for everyday use and office wear.</p>
      <ul>
        <li>50ml refill option</li>
        <li>Warm, fresh notes</li>
        <li>Quick bottle top-up</li>
      </ul>
      <div class="refill-price"><strong>KSh 30/ML</strong><span>From</span></div>
    </article>

    <article class="refill-card">
      <span class="refill-badge">Signature</span>
      <h3>Premium Evening Blend</h3>
      <p>Rich, elegant fragrance for events, dates and special occasions.</p>
      <ul>
        <li>80ml refill option</li>
        <li>Bold oud and spice</li>
        <li>Long-lasting aroma</li>
      </ul>
      <div class="refill-price"><strong>KSh 30/ML</strong><span>From</span></div>
    </article>

    <article class="refill-card">
      <span class="refill-badge">Fresh</span>
      <h3>Unisex Everyday Scent</h3>
      <p>Light and balanced fragrance for all-day comfort and freshness.</p>
      <ul>
        <li>30ml and 60ml sizes</li>
        <li>Fresh floral notes</li>
        <li>Portable and clean</li>
      </ul>
      <div class="refill-price"><strong>KSh 30/ML</strong><span>From</span></div>
    </article>
  </div>
</section>

<section class="section why-us">
  <div class="section-heading">
    <p class="tagline">WHY CHOOSE US?</p>
    <h2>Good Service, Every Visit</h2>
  </div>

  <div class="benefits">
    <div>
      <span>✓</span>
      <h3>Friendly Assistance</h3>
      <p>Helpful service for every client.</p>
    </div>

    <div>
      <span>✓</span>
      <h3>Clear Pricing</h3>
      <p>Confirm prices before work begins.</p>
    </div>

    <div>
      <span>✓</span>
      <h3>Convenience</h3>
      <p>Cyber services, Windows installation and fragrance refills in one place.</p>
    </div>
  </div>
</section>

<section class="contact-section" id="contact">
  <div class="contact-info">
    <p class="tagline" style="color:var(--gold)">GET IN TOUCH</p>
    <h2>How Can We Help You?</h2>
    <p>Send an enquiry and continue the conversation on WhatsApp.</p>
    <p>Location: Owour Church Junction</p>
    <p>Call: <a href="tel:+254769535087">0769 535 087</a></p>
    <p>Hours: Open daily, 7:00 AM–8:00 PM</p>
    
  </div>

  <form class="contact-form" id="contactForm">
    <h3>Send an Enquiry</h3>

    <label for="name">Your Name</label>
    <input type="text" id="name" placeholder="Enter your name" required>

    <label for="phone">Phone Number (optional)</label>
    <input type="tel" id="phone" placeholder="07XX XXX XXX">

    <label for="service">Select a Service</label>
    <select id="service" required>
      <option value="">Choose a service</option>
      <option>Printing and photocopying</option>
      <option>Online services</option>
      <option>Typing and scanning</option>
      <option>Design and binding</option>
      <option>Windows installation</option>
      <option>Perfume refill</option>
      <option>Other enquiry</option>
    </select>

    <label for="message">Your Message</label>
    <textarea id="message" rows="4"
      placeholder="Tell us what you need..." required></textarea>

    <button type="submit" class="btn">Send via WhatsApp ↗</button>
    <p id="formMessage" role="status"></p>
  </form>
</section>
</main>

<footer>
  <a href="#home" class="footer-logo">MASTERS CYBER</a>
  <p>Cyber services, Windows installation & perfume refills</p>
  <p>© <span id="year"></span> MASTERS Cyber. All rights reserved.</p>
</footer>

<a class="whatsapp-float"
   href="https://wa.me/254769535087"
   target="_blank"
   rel="noopener"
   aria-label="Chat with MASTERS Cyber on WhatsApp">W</a>

<script>
// Your business WhatsApp number.
// Kenyan format: 2547XXXXXXXX, digits only.
const BUSINESS_WHATSAPP = "254769535087";
const BUSINESS_DISPLAY_NUMBER = "0769535087";

// Mobile navigation
const menuToggle = document.getElementById("menuToggle");
const navigation = document.getElementById("navigation");

menuToggle.addEventListener("click", () => {
  const isOpen = navigation.classList.toggle("open");
  menuToggle.setAttribute("aria-expanded", String(isOpen));
  menuToggle.textContent = isOpen ? "×" : "☰";
});

navigation.querySelectorAll("a").forEach(link => {
  link.addEventListener("click", () => {
    navigation.classList.remove("open");
    menuToggle.setAttribute("aria-expanded", "false");
    menuToggle.textContent = "☰";
  });
});

document.addEventListener("keydown", event => {
  if (event.key === "Escape" && navigation.classList.contains("open")) {
    navigation.classList.remove("open");
    menuToggle.setAttribute("aria-expanded", "false");
    menuToggle.textContent = "☰";
    menuToggle.focus();
  }
});

const header = document.querySelector("header");
const updateHeader = () => header.classList.toggle("scrolled", window.scrollY > 12);
updateHeader();
window.addEventListener("scroll", updateHeader, { passive: true });

const observedSections = [...document.querySelectorAll("section[id]")];
const navLinks = [...navigation.querySelectorAll("a")];

if ("IntersectionObserver" in window) {
  const sectionObserver = new IntersectionObserver(entries => {
    const visible = entries
      .filter(entry => entry.isIntersecting)
      .sort((a, b) => b.intersectionRatio - a.intersectionRatio)[0];

    if (!visible) return;
    navLinks.forEach(link => {
      link.classList.toggle(
        "active",
        link.getAttribute("href") === `#${visible.target.id}`
      );
    });
  }, { rootMargin: "-20% 0px -65%", threshold: [0.05, 0.25, 0.5] });

  observedSections.forEach(section => sectionObserver.observe(section));
}

// Automatically update the copyright year
document.getElementById("year").textContent =
  new Date().getFullYear();

// Select the service automatically when clicked
const serviceSelect = document.getElementById("service");

document.querySelectorAll("[data-service]").forEach(link => {
  link.addEventListener("click", () => {
    serviceSelect.value = link.dataset.service;
  });
});

// Contact form: prepare a WhatsApp message
document.getElementById("contactForm").addEventListener("submit", event => {
  event.preventDefault();

  const name = document.getElementById("name").value.trim();
  const phone = document.getElementById("phone").value.trim();
  const service = serviceSelect.value;
  const message = document.getElementById("message").value.trim();
  const feedback = document.getElementById("formMessage");

  feedback.textContent = "";
  feedback.classList.remove("success");

  if (!name || !service || !message) {
    feedback.textContent = "Please complete all required fields.";
    return;
  }

  if (!/^\d{10,15}$/.test(BUSINESS_WHATSAPP) ||
      BUSINESS_WHATSAPP === "25470000000") {
    feedback.textContent =
      "Please add your real business WhatsApp number in the JavaScript section.";
    return;
  }
  
  const whatsappMessage = [
    "Hello! I found your website and would like to enquire.",
    "",
    `Name: ${name}`,
    phone ? `My phone: ${phone}` : "",
    `Service: ${service}`,
    `Message: ${message}`
  ].filter(Boolean).join("\n");

  const whatsappNumber = BUSINESS_WHATSAPP.replace(/\D/g, "");
  const url = `https://wa.me/${whatsappNumber}?text=${encodeURIComponent(whatsappMessage)}`;

  const newWindow = window.open(url, "_blank", "noopener,noreferrer");
  if (!newWindow) {
    window.location.href = url;
  }
});
</script>

</body>
</html>
