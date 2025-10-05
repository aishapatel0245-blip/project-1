# project-1
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meet the Team - Logos</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: Georgia, serif;
            background-color: #F2E5B3;
            color: #5A4A42;
            line-height: 1.6;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        /* Header Section */
        .header {
            text-align: center;
            padding: 60px 20px;
        }
        .header h1 {
            font-family: 'Brush Script MT', cursive;
            font-size: 42px;
            color: #A96255;
            margin-bottom: 20px;
        }
        .header p {
            font-size: 18px;
            color: #5A4A42;
            font-weight: bold;
        }
        .header p strong {
            color: #A96255;
        }
        .header p em {
            font-style: italic;
        }
        /* Team Grid */
        .team-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 30px;
            margin: 60px 0;
        }
        .team-card {
            background-color: #F8F4F0;
            border-radius: 10px;
            padding: 20px;
            text-align: center;
            box-shadow: 2px 2px 8px rgba(169, 98, 85, 0.1);
            transition: transform 0.3s ease;
        }
        .team-card:hover {
            transform: translateY(-5px);
        }
        .team-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 10px;
            margin-bottom: 15px;
        }
        .team-card h3 {
            font-family: Georgia, serif;
            font-size: 20px;
            color: #A96255;
            font-weight: bold;
            margin: 10px 0;
        }
        .team-card h4 {
            font-family: Georgia, serif;
            font-size: 16px;
            color: #6F927F;
            margin: 5px 0;
        }
        .team-card p.description {
            font-family: Georgia, serif;
            font-size: 14px;
            color: #7A6A62;
            font-style: italic;
            margin: 10px 0;
        }
        .team-card p.quote {
            font-family: Georgia, serif;
            font-size: 13px;
            color: #8B7D76;
            font-style: italic;
            margin-top: 15px;
            border-top: 1px solid #E8DECD;
            padding-top: 10px;
        }
        /* Adjust for last row: 2 centered */
        .team-grid > div:nth-child(7),
        .team-grid > div:nth-child(8) {
            grid-column: 2 / span 2;
            margin: 0 auto;
            width: calc(100% / 3 * 2 - 30px);
        }
        /* Lists Section */
        .lists-section {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            margin: 60px 0;
            background-color: #F6F0E8;
            padding: 40px;
            border-radius: 10px;
        }
        .lists-section h2 {
            font-family: Georgia, serif;
            font-size: 20px;
            color: #A96255;
            font-weight: bold;
            text-align: center;
            margin-bottom: 20px;
        }
        .lists-section ul {
            list-style: none;
            padding: 0;
        }
        .lists-section li {
            font-family: Georgia, serif;
            font-size: 16px;
            color: #5A4A42;
            margin-bottom: 10px;
            padding-left: 20px;
            position: relative;
        }
        .unordered li::before {
            content: "●";
            color: #6F927F;
            font-size: 18px;
            position: absolute;
            left: 0;
        }
        .ordered {
            counter-reset: list-counter;
        }
        .ordered li {
            counter-increment: list-counter;
        }
        .ordered li::before {
            content: counter(list-counter) ".";
            color: #A96255;
            font-weight: bold;
            position: absolute;
            left: 0;
        }
        /* Footer */
        .footer {
            background-color: #E8D8C8;
            text-align: center;
            padding: 30px;
            font-family: Georgia, serif;
            font-size: 14px;
            color: #7A6A62;
            margin-top: 60px;
        }
        .footer a {
            color: #A96255;
            text-decoration: none;
        }
        .footer a:hover {
            text-decoration: underline;
        }
        /* Responsive */
        @media (max-width: 768px) {
            .team-grid {
                grid-template-columns: 1fr;
            }
            .team-grid > div:nth-child(7),
            .team-grid > div:nth-child(8) {
                grid-column: 1;
                width: 100%;
            }
            .lists-section {
                grid-template-columns: 1fr;
                gap: 20px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header -->
        <section class="header">
            <h1>Meet Our Visionary Team</h1>
            <p>At <strong>Logos</strong>, we believe books are more than pages—they're <em>portals to new worlds</em>, conversations with great minds, and the binding that connects our community. We're not just selling books; we're cultivating readers, sparking imaginations, and writing our own story—<em>one chapter at a time</em>. Meet the passionate team who make our vision possible.</p>
        </section>

        <!-- Team Grid -->
        <section class="team-grid">
            <!-- Sophia -->
            <div class="team-card">
                <img src="https://images.unsplash.com/photo-1559757148-5c350d0d3c56?ixlib=rb-4.0.3&auto=format&fit=crop&w=300&h=200&q=80" alt="Sophia Hartman">
                <h3>Sophia Hartman</h3>
                <h4>Founder & CEO</h4>
                <p class="description">Visionary leader, guiding strategy and growth.</p>
                <p class="quote">Favorite Quote: “Do not go where the path may lead, go instead where there is no path and leave a trail.” — Ralph Waldo Emerson, <em>Essays</em> (1841)</p>
            </div>

            <!-- Max -->
            <div class="team-card">
                <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?ixlib=rb-4.0.3&auto=format&fit=crop&w=300&h=200&q=80" alt="Max Rivera">
                <h3>Max Rivera</h3>
                <h4>Creative Director</h4>
                <p class="description">Shapes the brand’s style, bold and imaginative.</p>
                <p class="quote">Favorite Quote: “Imagination is the only weapon in the war against reality.” — Lewis Carroll, <em>Alice’s Adventures in Wonderland</em> (1865)</p>
            </div>

            <!-- Emma -->
            <div class="team-card">
                <img src="https://images.unsplash.com/photo-1494790108755-2616b612b786?ixlib=rb-4.0.3&auto=format&fit=crop&w=300&h=200&q=80" alt="Emma Hartman-Zhang">
                <h3>Emma Hartman-Zhang</h3>
                <h4>Head Editor</h4>
                <p class="description">Detail-focused, ensures stories shine and flow.</p>
                <p class="quote">Favorite Quote: “It is our choices that show what we truly are, far more than our abilities.” — J.K. Rowling, <em>Harry Potter and the Chamber of Secrets</em> (1998)</p>
            </div>

            <!-- Lila -->
            <div class="team-card">
                <img src="https://images.unsplash.com/photo-1438761681033-6461ffad8d80?ixlib=rb-4.0.3&auto=format&fit=crop&w=300&h=200&q=80" alt="Lila Thompson">
                <h3>Lila Thompson</h3>
                <h4>Marketing & Communications Lead</h4>
                <p class="description">Bubbly and creative, shares stories with the world.</p>
                <p class="quote">Favorite Quote: “Sometimes, the hardest part isn’t letting go but learning to start over.” — Nicholas Sparks, <em>Safe Haven</em> (2010)</p>
            </div>

            <!-- Javier -->
            <div class="team-card">
                <img src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?ixlib=rb-4.0.3&auto=format&fit=crop&w=300&h=200&q=80" alt="Javier Hartman">
                <h3>Javier Hartman</h3>
                <h4>Community & Events Coordinator</h4>
                <p class="description">Connects people, plans events, builds community.</p>
                <p class="quote">Favorite Quote: “Happiness is only real when shared.” — Jon Krakauer, <em>Into the Wild</em> (1996)</p>
            </div>

            <!-- Claire -->
            <div class="team-card">
                <img src="https://images.unsplash.com/photo-1552664730-d307ca884978?ixlib=rb-4.0.3&auto=format&fit=crop&w=300&h=200&q=80" alt="Claire Hartman">
                <h3>Claire Hartman</h3>
                <h4>Operations Manager</h4>
                <p class="description">Keeps things organized, reliable, efficient.</p>
                <p class="quote">Favorite Quote: “The world only spins forward.” — Tony Kushner, <em>Angels in America</em> (1992; HBO adaptation revived 2018)</p>
            </div>

            <!-- Ethan -->
            <div class="team-card">
                <img src="https://images.unsplash.com/photo-1506784367992-9bc7a9cc2d0f?ixlib=rb-4.0.3&auto=format&fit=crop&w=300&h=200&q=80" alt="Ethan Brooks">
                <h3>Ethan Brooks</h3>
                <h4>Graphic / Visual Designer</h4>
                <p class="description">Trendy, creative, brings ideas to life visually.</p>
                <p class="quote">Favorite Quote: “One must always be careful of books, and what is inside them, for words have the power to change us.” — Cassandra Clare, <em>Clockwork Angel</em> (2010)</p>
            </div>

            <!-- Mr. Darcy -->
            <div class="team-card">
                <img src="https://images.unsplash.com/photo-1543466835-00a7907e9de1?ixlib=rb-4.0.3&auto=format&fit=crop&w=300&h=200&q=80" alt="Mr. Darcy Hartman">
                <h3>Mr. Darcy Hartman</h3>
                <h4>Head of Cuddles & Snacks</h4>
                <p class="description">Keeps spirits high, tests comfy chairs, approves all nap locations.</p>
                <p class="quote">Favorite Book Quote: “I can’t read, I’m a dog… but I love all the smells of books!”</p>
            </div>
        </section>

        <!-- Lists -->
        <section class="lists-section">
            <div class="unordered">
                <h2>Our Core Values:</h2>
                <ul>
                    <li>Curiosity First.</li>
                    <li>The Reader is Always Right.</li>
                    <li>Honesty in Every Sentence.</li>
                    <li>Respect the Deadline.</li>
                </ul>
            </div>
            <div class="ordered">
                <h2>Why Join Our Family?</h2>
                <ol>
                    <li>Curious minds with a strong work ethic.</li>
                    <li>Your boss brings in epic homemade cookies.</li>
                    <li>Our team WhatsApp is mostly dog pictures.</li>
                    <li>We need people who finish what they start.</li>
                </ol>
            </div>
        </section>
    </div>

    <!-- Footer -->
    <footer class="footer">
        <p>Connect with our family: <a href="mailto:team@logosbookstore.com">team@logosbookstore.com</a> | <a href="#">Our Partners</a> | <a href="family-story.pdf" download>Family Story PDF</a> | Last chapter updated: <span id="last-updated"></span></p>
    </footer>

    <script>
        document.getElementById('last-updated').textContent = new Date().toLocaleDateString();
    </script>
</body>
</html>
