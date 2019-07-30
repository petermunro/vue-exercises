# Conditional Rendering

The data (below) now shows a `balanceOutstanding` field.

1. For clients that are in arrears (ie a non-zero balance), display a message "In arrears".

2. For clients that have a zero balance, display the message "Send a gift".

---

      let clients = [
        {
          name: "Dibbert Koepp",
          city: "Carmelaberg",
          country: "Seychelles",
          balanceOutstanding: 0
        },
        {
          name: "Schinner and Sons",
          city: "Marcelinoland",
          country: "Mozambique",
          balanceOutstanding: 4000
        },
        {
          name: "Walsh Inc",
          city: "New Clyde",
          country: "Saint Helena",
          balanceOutstanding: 200
        },
        {
          name: "Donnelly Group",
          city: "North Carolineberg",
          country: "Iceland",
          balanceOutstanding: 560
        },
        {
          name: "Kub LLC",
          city: "Strosinland",
          country: "Panama",
          balanceOutstanding: 0
        },
        {
          name: "Okuneva Krajcik",
          city: "Jacobston",
          country: "Somalia",
          balanceOutstanding: 120
        },
        {
          name: "Wolff, Braun and Hettinger",
          city: "Port Horace",
          country: "Mozambique",
          balanceOutstanding: 40
        }
      ];
