<h2 class="c-project-heading--task">Arrange facts with grids</h2>

Turn your facts into image cards arranged in a grid.

--- task ---

Open `index.html` and add classes so your fact cards can be laid out and styled.

<div class="c-project-code">

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 25
line_highlights: 29-48
---
    <main>
      <section>
        <h1>Welcome to Antarctica!</h1>
        <h1>Hover on the cards below to read some facts about Antarctica</h1>
        <div class="fact-holder">
          <span class="fact-card sun">
            <p class="fact">
              Antarctica is the coldest continent, but it is also the driest! On average, there is just 200mm (8 inches) of precipitation a year, the majority of it along the coast.
            </p>
          </span>
          <span class="fact-card discovery">
            <p class="fact">
              The continent is thought to have been discovered relatively late in human history. In 1820, Fabian Gottlieb von Bellingshausen and Mikhail Lazarev lead a Russian expedition to prove the exsistence of Antarctica and were probably the first to see the ice shelves. 
            </p>
          </span>
          <span class="fact-card explorers">
            <p class="fact">
              Who first set foot on the continent? The first documented and confirmed landing was a crew led by Norwegian Leonard Kristensen at Cape Adare.
            </p>
          </span>
          <span class="fact-card ownership">
            <p class="fact">
              Antarctica is governed by the Antarctic Treaty. The Treaty now has 56 supporting nations, 29 of which are considered “Consultative Parties” and are actively involved in decision-making.
            </p>
          </span>
        </div>
      </section>
    </main>
--- /code ---

</div>

--- /task ---

--- task ---

**Test:** Run the Home page and check you can see four fact “cards” arranged in a grid.

--- /task ---