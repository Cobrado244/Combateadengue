<!DOCTYPE html>
<title>Combate à Dengue - Prevenção, Sintomas e Cuidados</title> <style> * { margin: 0; padding: 0; box-sizing: border-box; }
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
    <title>Combate à Dengue - Prevenção, Sintomas e Cuidados</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', 'Roboto', system-ui, -apple-system, 'Helvetica Neue', sans-serif;
            background: linear-gradient(145deg, #eaf7e6 0%, #d4e9d0 100%);
            color: #1e2f2c;
            line-height: 1.5;
            scroll-behavior: smooth;
        }

        /* Container principal responsivo */
        .container {
            max-width: 1300px;
            margin: 0 auto;
            padding: 2rem 1.5rem;
        }

        /* Header com imagem temática */
        .hero {
            background: linear-gradient(135deg, #0e4b3a, #1d6b54);
            border-radius: 2.5rem;
            padding: 3rem 2rem;
            margin-bottom: 3rem;
            box-shadow: 0 20px 35px -12px rgba(0, 0, 0, 0.25);
            text-align: center;
            color: white;
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: "🦟";
            font-size: 14rem;
            position: absolute;
            bottom: -40px;
            right: -30px;
            opacity: 0.12;
            pointer-events: none;
            transform: rotate(10deg);
        }

        .hero h1 {
            font-size: 2.8rem;
            font-weight: 800;
            letter-spacing: -0.01em;
            margin-bottom: 0.5rem;
            text-shadow: 2px 2px 6px rgba(0,0,0,0.2);
        }

        .hero p {
            font-size: 1.3rem;
            max-width: 700px;
            margin: 1rem auto 0;
            opacity: 0.95;
            font-weight: 500;
        }

        .hero-badge {
            background-color: #ffd966;
            display: inline-block;
            padding: 0.5rem 1.2rem;
            border-radius: 100px;
            color: #1e4d3c;
            font-weight: bold;
            font-size: 0.9rem;
            margin-bottom: 1rem;
            letter-spacing: 0.5px;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
        }

        /* grade cards principais */
        .grid-highlight {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 2rem;
            margin-bottom: 3rem;
        }

        .card {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(2px);
            border-radius: 2rem;
            padding: 1.8rem;
            box-shadow: 0 20px 30px -12px rgba(0, 0, 0, 0.1);
            transition: transform 0.25s ease, box-shadow 0.3s;
            border: 1px solid rgba(160, 200, 140, 0.5);
        }

        .card:hover {
            transform: translateY(-6px);
            box-shadow: 0 28px 36px -14px rgba(0, 32, 0, 0.2);
            background: #ffffff;
        }

        .card-icon {
            font-size: 2.8rem;
            background: #e2f0dd;
            display: inline-block;
            padding: 0.6rem;
            border-radius: 2rem;
            margin-bottom: 1.2rem;
        }

        .card h2 {
            font-size: 1.8rem;
            margin-bottom: 1rem;
            color: #145c44;
            border-left: 5px solid #f9b81b;
            padding-left: 0.8rem;
        }

        .card p, .card li {
            color: #2c423d;
            font-size: 1rem;
        }

        .card ul, .card ol {
            padding-left: 1.4rem;
            margin: 1rem 0;
        }

        .card li {
            margin: 0.6rem 0;
        }

        /* seção destacada de sintomas e ação */
        .sintomas-wrapper {
            background: #fff6e8;
            border-radius: 2rem;
            padding: 2.2rem;
            margin: 2.5rem 0;
            box-shadow: 0 12px 20px rgba(0, 0, 0, 0.05);
            border-left: 12px solid #e67e22;
        }

        .sintomas-wrapper h2 {
            font-size: 2rem;
            margin-bottom: 1rem;
            display: flex;
            align-items: center;
            gap: 12px;
            color: #b85c00;
        }

        .sintomas-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 1.5rem;
            margin: 1.5rem 0;
        }

        .sintoma-item {
            background: white;
            flex: 1 1 200px;
            padding: 1rem;
            border-radius: 1.5rem;
            text-align: center;
            font-weight: 600;
            box-shadow: 0 4px 8px rgba(0,0,0,0.05);
            border-bottom: 4px solid #ffb347;
        }

        .sintoma-item span {
            font-size: 2rem;
            display: block;
            margin-bottom: 0.4rem;
        }

        .acao-rapida {
            background: #eef4ec;
            border-radius: 1.5rem;
            padding: 1.5rem;
            margin-top: 1rem;
        }

        .btn-alerta {
            background-color: #d9534f;
            color: white;
            border: none;
            padding: 0.8rem 1.8rem;
            border-radius: 3rem;
            font-weight: bold;
            font-size: 1rem;
            cursor: pointer;
            transition: 0.2s;
            display: inline-block;
            margin-top: 0.8rem;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
        }

        .btn-alerta:hover {
            background-color: #c9302c;
            transform: scale(1.02);
        }

        /* lista de cuidados profundos */
        .prevencao-detalhada {
            background: #eef2ea;
            border-radius: 2rem;
            padding: 2rem;
            margin: 2rem 0;
        }

        .prevencao-detalhada h3 {
            font-size: 1.7rem;
            color: #1b5e3f;
            margin-bottom: 1rem;
        }

        .grid-dicas {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 1.4rem;
            margin-top: 1.2rem;
        }

        .dica-card {
            background: white;
            border-radius: 1.2rem;
            padding: 1.2rem;
            box-shadow: 0 2px 8px rgba(0,0,0,0.05);
            transition: all 0.2s;
        }

        .dica-card strong {
            display: block;
            font-size: 1.2rem;
            color: #1d734f;
            margin-bottom: 0.5rem;
        }

        footer {
            background-color: #1b3b32;
            color: #d4e2d0;
            text-align: center;
            padding: 2rem 1rem;
            border-radius: 2rem 2rem 0 0;
            margin-top: 3rem;
            font-size: 0.9rem;
        }

        a {
            color: #ffc857;
            text-decoration: none;
        }

        @media (max-width: 700px) {
            .hero h1 {
                font-size: 2rem;
            }
            .container {
                padding: 1rem;
            }
            .card h2 {
                font-size: 1.5rem;
            }
        }

        .aviso-saude {
            background: #fef1e0;
            border-radius: 1rem;
            padding: 1rem;
            font-size: 0.9rem;
            margin-top: 1rem;
            border-left: 6px solid #f0ad4e;
        }
    </style>
</head>
<body>
<div class="container">
    <div class="hero">
        <div class="hero-badge">⚠️ Alerta epidemiológico</div>
        <h1>Dengue: proteção, sintomas e ação imediata</h1>
        <p>Informações completas e imersivas para combater o mosquito Aedes aegypti, prevenir a doença e saber exatamente o que fazer ao surgirem os primeiros sinais.</p>
    </div>

    <!-- cards de visão geral: prevenção + cuidados + o que fazer -->
    <div class="grid-highlight">
        <div class="card">
            <div class="card-icon">🛡️🧹</div>
            <h2>Prevenção & Cuidados Essenciais</h2>
            <p>A eliminação de criadouros do mosquito transmissor é a principal arma contra a dengue. Pequenas atitudes no dia a dia salvam vidas:</p>
            <ul>
                <li>✔️ Mantenha caixas d'água, tonéis e barris bem tampados.</li>
                <li>✔️ Limpe calhas, lajes e ralos, removendo folhas e acúmulo de água.</li>
                <li>✔️ Guarde pneus em locais cobertos ou faça furos para drenagem.</li>
                <li>✔️ Lave semanalmente os potes de água dos animais com escova e sabão.</li>
                <li>✔️ Coloque areia nos pratos de vasos de plantas.</li>
                <li>✔️ Trate piscinas com cloro e mantenha-as cobertas quando não usadas.</li>
                <li>✔️ Use telas de proteção em portas e janelas, além de repelentes registrados.</li>
            </ul>
            <div class="aviso-saude">
                💡 <strong>Dica extra:</strong> Inspecione quintais, garagens e áreas de serviço ao menos uma vez por semana. O ovo do Aedes resiste por mais de um ano mesmo em ambiente seco!
            </div>
        </div>

        <div class="card">
            <div class="card-icon">🤒🔍</div>
            <h2>Sintomas: fique de olho!</h2>
            <p>A dengue pode ser assintomática ou evoluir com sinais que merecem atenção imediata. Conheça os principais sintomas e saiba quando agir:</p>
            <ul>
                <li>🔥 <strong>Febre alta</strong> (39°C a 40°C) de início repentino.</li>
                <li>🤕 <strong>Dor de cabeça intensa</strong> e dor atrás dos olhos.</li>
                <li>🦴 <strong>Dores no corpo e articulações</strong> (quebranto).</li>
                <li>🤢 Náuseas, vômitos ou diarreia.</li>
                <li>🩸 Manchas vermelhas na pele (exantema), coceira.</li>
                <li>😴 Cansaço extremo e prostração.</li>
            </ul>
            <p><strong>⚠️ Sinais de alarme (dengue grave):</strong> dor abdominal forte, vômitos persistentes, sangramento nasal ou gengival, tontura, sonolência, extremidades frias. <u>Busque atendimento urgente!</u></p>
        </div>

        <div class="card">
            <div class="card-icon">🏥💊</div>
            <h2>O que fazer após os sintomas?</h2>
            <p>Se você ou alguém próximo apresentar sintomas suspeitos, siga estas orientações fundamentais:</p>
            <ol>
                <li><strong>1. Procure uma unidade de saúde</strong> imediatamente. Não se automedique!</li>
                <li><strong>2. Evite medicamentos à base de ácido acetilsalicílico (aspirina)</strong> ou anti-inflamatórios, pois aumentam risco de sangramentos. Prefira dipirona ou paracetamol apenas com orientação médica.</li>
                <li><strong>3. Hidrate-se bastante</strong> – água, soro caseiro, água de coco, sucos naturais (sem açúcar).</li>
                <li><strong>4. Repouso absoluto</strong> é essencial para recuperação.</li>
                <li><strong>5. Monitore sinais de alarme</strong> especialmente entre o 3º e 7º dia, mesmo que a febre diminua.</li>
                <li><strong>6. Siga rigorosamente as recomendações médicas</strong> e realize exames de sangue se solicitado.</li>
            </ol>
            <div class="aviso-saude">
                🚨 <strong>NÃO tome remédios por conta própria!</strong> Ibuprofeno, nimesulida e aspirina podem agravar complicações hemorrágicas.
            </div>
        </div>
    </div>

    <!-- Seção especial: sintomas + ação imersiva -->
    <div class="sintomas-wrapper">
        <h2>📋 Sintomas em detalhe — o que monitorar no seu corpo?</h2>
        <p>A dengue clássica se manifesta de forma aguda. Fique atento aos seguintes sinais e mantenha um diário dos sintomas nas primeiras 48 horas. Em crianças e idosos, os sinais podem ser mais discretos, mas a febre e a prostração são marcantes.</p>
        <div class="sintomas-grid">
            <div class="sintoma-item"><span>🌡️</span> Febre alta (39°C+)</div>
            <div class="sintoma-item"><span>👁️</span> Dor retro-ocular</div>
            <div class="sintoma-item"><span>🤧</span> Manchas vermelhas</div>
            <div class="sintoma-item"><span>🦵</span> Dores musculares fortes</div>
            <div class="sintoma-item"><span>🤢</span> Náuseas / vômitos</div>
            <div class="sintoma-item"><span>🩸</span> Sangramentos leves (gengiva/nariz)</div>
        </div>
        <div class="acao-rapida">
            <h3 style="margin-top:0;">🆘 Protocolo de emergência para suspeita de dengue</h3>
            <p><strong>Assim que surgirem sintomas compatíveis:</strong> dirija-se à unidade de saúde mais próxima para testagem e acompanhamento. Nunca ignore dores abdominais intensas ou vômitos frequentes. A dengue pode evoluir rapidamente para formas graves — hidratação venosa e monitoramento são cruciais.</p>
            <button class="btn-alerta" id="alertBtn">📢 Lembrete de hidratação e cuidados</button>
            <div id="alertMessage" style="margin-top: 12px; font-weight: bold;"></div>
        </div>
    </div>

    <!-- Prevenção profunda: cuidados diários e rotina de combate -->
    <div class="prevencao-detalhada">
        <h3>🧹 Prevenção profunda: como eliminar criadouros e proteger sua família</h3>
        <p>O Aedes aegypti se prolifera em qualquer recipiente que acumule água parada, até mesmo tampinhas de garrafa. Uma rotina semanal de inspeção reduz drasticamente a infestação. Além disso, use barreiras físicas e comunitárias.</p>
        <div class="grid-dicas">
            <div class="dica-card"><strong>🏠 Dentro de casa</strong> Verifique atrás da geladeira, bandejas de ar-condicionado, umidificadores e plantas aquáticas. Troque a água dos vasos de flores por areia úmida.</div>
            <div class="dica-card"><strong>🚮 Lixo e recicláveis</strong> Mantenha sacos de lixo bem fechados e latas de lixo tampadas. Garrafas PET devem ser armazenadas com boca para baixo ou em local coberto.</div>
            <div class="dica-card"><strong>🍃 Pátios e jardins</strong> Elimine folhas acumuladas, limpe a bandeja externa do ar-condicionado, cubra piscinas infantis após uso e fure pneus velhos.</div>
            <div class="dica-card"><strong>🐶 Cuidado com animais</strong> Bebedouros de pets: limpe com escova e troque a água diariamente. Ralos pouco usados: coloque uma tela ou jogue água sanitária semanalmente.</div>
            <div class="dica-card"><strong>🌧️ Calhas e lajes</strong> Após chuvas, verifique se não há acúmulos em coberturas e calhas entupidas. Use larvicidas biológicos (Bti) onde não é possível eliminar a água.</div>
            <div class="dica-card"><strong>🧴 Proteção individual</strong> Use repelentes à base de DEET, Icaridina ou IR3535, principalmente ao amanhecer e entardecer. Instale telas mosquiteiras e utilize roupas claras que cubram pernas e braços.</div>
        </div>
        <div class="aviso-saude" style="margin-top: 1.5rem;">
            🧑‍🤝‍🧑 <strong>Engajamento comunitário:</strong> Mobilize vizinhos para mutirões de limpeza. A dengue não respeita muros — um depósito de água parada em uma resid vizinha pode colocar todo o quarteirão em risco.
        </div>
    </div>

    <!-- Perguntas frequentes e dicas adicionais (texto imersivo) -->
    <div style="background: #f9faf6; border-radius: 2rem; padding: 2rem; margin: 1.5rem 0;">
        <h3 style="color:#145c44; font-size: 1.8rem; margin-bottom: 0.5rem;">❓ Dúvidas comuns sobre dengue e prevenção</h3>
        <div style="display: flex; flex-direction: column; gap: 1rem;">
            <p><strong>🔹 Dengue pode ser transmitida de pessoa para pessoa?</strong> Não, a transmissão ocorre exclusivamente pela picada da fêmea do Aedes aegypti infectado. Não há contágio direto entre humanos.</p>
            <p><strong>🔹 Quem já teve dengue pode pegar novamente?</strong> Sim. Existem quatro sorotipos diferentes do vírus (DENV-1,2,3,4). Uma infecção confere imunidade somente para aquele sorotipo específico. Uma segunda infecção por outro tipo pode aumentar o risco de dengue grave, por isso a prevenção é ainda mais crucial.</p>
            <p><strong>🔹 Vacina contra dengue: já está disponível?</strong> O Brasil oferece a vacina Qdenga em campanhas para público-alvo (crianças e adolescentes de 10 a 14 anos) em algumas regiões. Procure o posto de saúde para informações sobre elegibilidade. A vacinação não elimina a necessidade de eliminar criadouros.</p>
            <p><strong>🔹 É verdade que cloro e água sanitária matam as larvas?</strong> Sim, mas a solução mais segura e efetiva é eliminar o ambiente aquático. Caso o recipiente não possa ser removido (ex: piscina, cisterna), adicione cloro regularmente ou utilize larvicida aprovado.</p>
        </div>
    </div>

    <!-- Bloco de orientação pós-sintomas e cuidados extensivos -->
    <div style="background: #ddebe2; border-radius: 2rem; padding: 2rem; margin: 1.5rem 0;">
        <h3 style="font-size: 1.7rem; color:#1d523f;">🩺 Diagnóstico e conduta médica: o que esperar?</h3>
        <p>Após buscar atendimento com suspeita de dengue, o profissional pode solicitar exame de sangue (hemograma, pesquisa de antígeno NS1 ou sorologia). O tratamento é basicamente de suporte: hidratação oral ou intravenosa, repouso e medicação para febre/dor com orientação médica. Nos casos de sinais de alarme, a internação é necessária para acompanhamento de plaquetas e prevenção de choque.</p>
        <p><strong>Importante:</strong> Durante a recuperação, mantenha a ingestão de líquidos mesmo após a febre ceder. O período de convalescença pode durar até 10 dias com cansaço persistente.</p>
        <div style="display: flex; flex-wrap: wrap; gap: 1rem; margin: 1.2rem 0;">
            <span style="background: #fff2db; border-radius: 3rem; padding: 0.4rem 1rem;">✅ Hidratação contínua</span>
            <span style="background: #fff2db; border-radius: 3rem; padding: 0.4rem 1rem;">✅ Repouso prolongado</span>
            <span style="background: #fff2db; border-radius: 3rem; padding: 0.4rem 1rem;">✅ Evitar esforço físico</span>
            <span style="background: #fff2db; border-radius: 3rem; padding: 0.4rem 1rem;">✅ Não usar ácido acetilsalicílico</span>
        </div>
    </div>

    <footer>
        <p>🚨 Ministério da Saúde • Combate à Dengue • Informações baseadas em diretrizes da OMS e do Programa Nacional de Controle da Dengue</p>
        <p style="margin-top: 12px;">📞 Disque Saúde 136 para dúvidas e orientações • Em caso de emergência, procure o SAMU 192 ou UPA mais próxima</p>
        <p style="margin-top: 16px;">🕯️ A prevenção é de todos. Elimine focos, salve vidas.</p>
    </footer>
</div>

<script>
    // interatividade educativa sutil - botão de alerta com dicas preventivas e conduta pós-sintomas
    const alertBtn = document.getElementById('alertBtn');
    const alertMsgDiv = document.getElementById('alertMessage');

    alertBtn.addEventListener('click', () => {
        alertMsgDiv.innerHTML = '💧 <strong>Lembrete essencial:</strong> Em caso de sintomas (febre, dores, manchas), procure atendimento, hidrate-se com frequência e NÃO tome anti-inflamatórios! Para prevenção, inspecione sua casa agora mesmo e elimine qualquer água parada. 🦟🚫';
        alertMsgDiv.style.background = '#fff3cd';
        alertMsgDiv.style.padding = '12px 18px';
        alertMsgDiv.style.borderRadius = '50px';
        alertMsgDiv.style.border = '1px solid #ffe0a3';
        alertMsgDiv.style.marginTop = '12px';
        setTimeout(() => {
            // opcional: apaga ou mantém visível, mas mantemos para destaque imersivo
        }, 200);
        // feedback visual adicional
        alertBtn.innerText = '✅ Lembrete enviado! Proteja-se.';
        setTimeout(() => {
            alertBtn.innerText = '📢 Lembrete de hidratação e cuidados';
        }, 4000);
    });
</script>
</body>
</html>
