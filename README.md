# timetablecreation
School Timetable Implementation Guide
####HTML Structure

We will use `<div>` elements to represent the table, rows, and cells. Classes will help us style them with CSS

`<div class="grid-table">`
  
  
 `<div class="grid-row header">`
 
    `<div class="grid-cell">Name</div>`
    
    `<div class="grid-cell">Age</div>`
    
    `<div class="grid-cell">Country</div>`
    
  `</div>`

  `<!-- Data Row 1 -->`
  
  `<div class="grid-row">`
  
    `<div class="grid-cell">Alice</div>`
    
    `<div class="grid-cell">25</div>`
    
    `<div class="grid-cell">Kenya</div>`
    
  `</div>`

  `<!-- Data Row 2 -->`
  `<div class="grid-row">`
  
    `<div class="grid-cell">Bob</div>`
    
    `<div class="grid-cell">30</div>`
    
    `<div class="grid-cell">South Africa</div>`
    
  `</div>`

#####CSS Styling Using Grid

.grid-table {

  display: grid;
  
  grid-template-columns: repeat(3, 1fr); /* 3 columns of equal width */
  
  gap: 1px; /* space between cells */
  
  background-color: #000; /* grid gap color */
}

/* Each cell */

.grid-cell {

  padding: 10px;
  
  background-color: #f0f0f0;
  
  border: 1px solid #ccc;
  
  text-align: center;
}

/* Header row */

.header .grid-cell {

  background-color: #4CAF50;
  
  color: white;
  
  font-weight: bold;
  }
  How It Works

.grid-table is a grid container with 3 columns (adjustable using grid-template-columns).

.grid-row is optional here because CSS Grid works on the container. But you can use it for styling rows differently if needed.

.grid-cell represents each cell.

.header gives a special style to the header row.
