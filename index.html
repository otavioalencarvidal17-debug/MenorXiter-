const { Client, GatewayIntentBits, EmbedBuilder, ActionRowBuilder, ButtonBuilder, ButtonStyle } = require('discord.js');
const express = require('express');

// --- SISTEMA PARA MANTER ONLINE ---
const app = express();
app.get('/', (req, res) => res.send('Bot de Fila Online!'));
app.listen(3000, () => console.log('Servidor de monitoramento rodando.'));

const client = new Client({
  intents: [
    GatewayIntentBits.Guilds,
    GatewayIntentBits.GuildMessages,
    GatewayIntentBits.MessageContent,
    GatewayIntentBits.GuildMembers
  ]
});

// --- CONFIGURAÇÃO ---
const TOKEN = "MTQ4MjQ5ODUzMzAzMzc3NTI5Nw.GcS4qX.IUFNVeY97DNXgqgpm3on93eYjTjQEPDqQjVApo"; 
const PIX_ADM = "SUA_CHAVE_PIX_AQUI";
const CARGO_GEL_ID = "ID_DO_CARGO_GEL";

client.once('ready', () => {
    console.log(`✅ Logado como ${client.user.tag}`);
});

client.on('messageCreate', async (message) => {
    if (message.content === '!setup') {
        if (!message.member.permissions.has('Administrator')) return;

        const embed = new EmbedBuilder()
            .setTitle('🎮 CENTRAL DE FILAS - MX STORE')
            .setDescription('Escolha sua modalidade abaixo:\n\n💎 **GEL:** Apenas elite.\n⚔️ **MISTA:** Todos os níveis.\n💰 **PIX:** Chave do ADM.')
            .setColor('#2f3136');

        const row = new ActionRowBuilder().addComponents(
            new ButtonBuilder().setCustomId('fila_gel').setLabel('Entrar GEL').setStyle(ButtonStyle.Primary),
            new ButtonBuilder().setCustomId('fila_mista').setLabel('Entrar Mista').setStyle(ButtonStyle.Success),
            new ButtonBuilder().setCustomId('pix').setLabel('Chave Pix').setStyle(ButtonStyle.Secondary)
        );

        message.channel.send({ embeds: [embed], components: [row] });
    }
});

client.on('interactionCreate', async (interaction) => {
    if (!interaction.isButton()) return;

    if (interaction.customId === 'pix') {
        return interaction.reply({ content: `💰 Chave Pix para apostados: \`${PIX_ADM}\``, ephemeral: true });
    }
    
    // Adicione aqui a lógica de armazenamento das listas se desejar salvar os nomes
    interaction.reply({ content: `✅ Você entrou na fila ${interaction.customId.replace('fila_', '')}!`, ephemeral: true });
});

client.login(TOKEN);
