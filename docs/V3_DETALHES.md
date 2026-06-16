# 🔧 V3 — Detalhes Técnicos da Bancada

## Visão Geral

Especificações completas da versão 3 da bancada de teste estático da Serra Rocketry. Esta versão utiliza cantoneira de aço com sistema de guia linear para medição precisa de empuxo em motores experimentais de médio porte.

---

## Especificações Estruturais

| Componente | Especificação |
|------------|---------------|
| Material da estrutura | Cantoneira de aço 1″ × 1/4″ |
| Pintura | Preto |
| Geometria | Retangular + mesa deslizante |

### Sistema de Guia Linear

| Componente | Especificação |
|------------|---------------|
| Eixo linear | ⌀12mm, comprimento 600mm |
| Rolamento | SC12UU (Pillow Block) |
| Tipo | Auto-alinhante (self-aligning) |
| Material do mancal | Alumínio fundido |
| Quantidade de eixos | 2 (paralelos, sem torção) |

O sistema de guia linear permite que o carro da bancada mova-se axialmente, transmitindo o empuxo do motor para a célula de carga sem cargas laterais parasitas. Os dois eixos paralelos garantem ausência de torção.

---

## Célula de carga

### Modelo

**SZ51X-500kg** — Fabricante: PESO

- Tipo: Viga em S (shear beam)
- Material: Aço inox
- Configuração: Cisalhamento entre dois suportes metálicos

### Especificações (Certificado de Calibração)

| Parâmetro | Valor |
|-----------|-------|
| Capacidade | 500 kgf (~4,9 kN) |
| Sensibilidade (full scale output) | 2,0 mV/V |
| Erro combinado | 0,02% F.S. |
| Não-linearidade | 0,02% F.S. |
| Repetibilidade | 0,01% F.S. |
| Histerese | 0,02% F.S. |
| Creep (30 min) | 0,02% F.S. |
| Sobrecarga segura | ±1,0% F.S. |
| Sobrecarga última | 150% F.S. |
| Impedância de entrada | 200 Ω |
| Impedância de saída | 350±5 Ω |
| Tensão de excitação | 5V (recomendado) / 12V (máx) |
| Temperatura compensada | -10 ~ +40°C |
| Temperatura de operação | -20 ~ +80°C |
| Aprovação QC | Pass 08 |

### Fiação

| Cor | Função |
|-----|--------|
| Vermelho | E+ (Excitação +) |
| Preto | E− (Excitação −) |
| Verde | S+ (Sinal +) |
| Branco | S− (Sinal −) |

---

## Resolução Estimada

Com o HX711 (24 bits) ou ADS1232 na aquisição:

- **Fundo de escala:** 4,9 kN (500 kgf)
- **Resolução estimada:** ~0,5 N
- **Cobertura:** Motores experimentais de médio porte (Dédalo, Thonyan)

---

## Fotos

### Célula de carga montada

![Célula de carga SZ51X-500kg](./imagens/v3_celula_carga.jpg)

Célula de carga tipo viga em S em aço inox, montada em configuração de cisalhamento entre dois suportes metálicos da estrutura pintada de preto.

### Certificado de calibração

![Certificado de calibração](./imagens/v3_certificado_calibracao.jpg)

Certificado do fabricante com especificações completas da SZ51X-500kg.

### Sistema de guia linear — montado

![Guia linear montado](./imagens/v3_guia_linear_montado.jpg)

Mancal SC12UU auto-alinhante em alumínio fundido, montado sobre eixo cromado de 12mm. O carrinho deslizante permite movimento axial, transmitindo empuxo sem cargas laterais.

### Rolamento SC12UU

![Rolamento SC12UU](./imagens/v3_rolamento_sc12uu.jpg)

Rolamento linear Pillow Block SC12UU isolado.
