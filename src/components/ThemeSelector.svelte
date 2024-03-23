<script>
    import { theme } from '../stores/themeStore';
  
    // This function could be enhanced to dynamically load the CSS file for the selected theme
    function changeTheme(newTheme) {
      theme.set(newTheme);
      // Assuming you have a mechanism to dynamically link to the CSS files based on the theme
    }
  </script>
  
  <select on:change="{(e) => changeTheme(e.target.value)}">
    <option value="crimson">Crimson</option>
    <option value="vintage">Vintage</option>
  </select>
  