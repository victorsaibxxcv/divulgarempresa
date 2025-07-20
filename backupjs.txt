
  
    // Array com os anúncios das empresas
    const empresas = [
      {
        nome: "Empresa Alpha",
        descricao: "Especializada em soluções tecnológicas para pequenas empresas.",
        imagem: "https://via.placeholder.com/300x200?text=Empresa+Alpha"
      },
      {
        nome: "Beta Logística",
        descricao: "Atuação nacional com foco em transporte sustentável e rastreável.",
        imagem: "https://via.placeholder.com/300x200?text=Beta+Logistica"
      },
      {
        nome: "Gamma Marketing",
        descricao: "Agência criativa voltada para marketing digital e redes sociais.",
        imagem: "https://via.placeholder.com/300x200?text=Gamma+Marketing"
      },
      {
        nome: "Delta Engenharia",
        descricao: "Projetos de construção civil com foco em inovação e sustentabilidade.",
        imagem: "https://via.placeholder.com/300x200?text=Delta+Engenharia"
      }
    ];

    const container = document.getElementById("empresa-container");

    empresas.forEach(empresa => {
      const card = document.createElement("div");
      card.className = "card";
      card.innerHTML = `
        <img src="${empresa.imagem}" alt="${empresa.nome}">
        <div class="card-content">
          <h2>${empresa.nome}</h2>
          <p>${empresa.descricao}</p>
        </div>
      `;
      container.appendChild(card);
    });
  
