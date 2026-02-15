<div align="center">
  <a href="https://git.io/streak-stats">
    <img id="streak-img" alt="GitHub Streak" />
  </a>
</div>

<script>
  const img = document.getElementById('streak-img');
  const user = "katto-1204";
  const width = 800;
  const height = 90;
  const borderRadius = 50;
  const hour = new Date().getHours();
  
  let theme = "rust-ferris-dark"; // default
  
  if (hour >= 6 && hour < 12) {          // Morning
    theme = "sea";
  } else if (hour >= 12 && hour < 18) {  // Afternoon
    theme = "git-dark";
  } else {                               // Evening/Night
    theme = "rust-ferris-dark";
  }

  img.src = `https://streak-stats.demolab.com?user=${user}&theme=${theme}&border_radius=${borderRadius}&mode=weekly&card_width=${width}&card_height=${height}`;
</script>
