[index.html](https://github.com/user-attachments/files/23997562/index.html)
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta name="description" content="AffinityPay - Remessas Brasil-Argentina 80% Mais Baratas">
    <title>SRT-BANK Finance</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
      tailwind.config = {
        darkMode: 'class',
        theme: {
          extend: {
            colors: {
              brand: {
                50: '#f5f3ff',
                100: '#ede9fe',
                200: '#ddd6fe',
                300: '#c4b5fd',
                400: '#a78bfa',
                500: '#8b5cf6',
                600: '#7c3aed',
                700: '#6d28d9',
                800: '#5b21b6',
                900: '#4c1d95',
                950: '#2e1065',
              }
            },
            animation: {
              'pulse-slow': 'pulse 3s cubic-bezier(0.4, 0, 0.6, 1) infinite',
            }
          }
        }
      }
    </script>
  </head>
  <body class="bg-slate-900 text-white">
    <div id="root"></div>
    <script type="module" src="/src/index.tsx"></script>
  </body>
</html>
