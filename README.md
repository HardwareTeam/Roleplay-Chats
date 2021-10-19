client.on('message', async message => {
    const Examplechannel = 'ChannelID'; 
    
    ///// Έτσι θα προσδιορίσεις ποιο κανάλι θέλεις το Bot σου να ενεργοποιητε και να τσεκάρει καθός γίνετε το message event!
    
  if (message.channel.id === Examplechannel) { /
  
  //// Το Bot σου θα τσεκάρει αμα το μήνυμα προέρχετε απο το κανάλι που έχεις δηλώσει παραπάνω
  
  if(!message.guild || message.author.bot) return; /
  
  //// Σημαντικό! Δεν θέλουμε να γίνετε λούπα οπότε πρέπει το Bot μας να ε΄λένχει αμα αυτος που έγραψε το μήνυμα ειναι άνθρωπος και όχι Bot!
      
if (message.attachments.size > 0) return; 

///// Άλλο ενα σημαντικό βήμα εδω προσδιορίζουμε το οτι το Bot να τρέξει το παρακάτω Script μονο και μονο αμα το περιεχόμενο ειναι ΜΗΝΥΜΑ και όχι φωτογραφ΄ία.


        const guildname = 'Dark Chat' 
        /// Το αλλάζεις με τα δικά σου θέλω
        const guild =  'https://tse1.mm.bing.net/th?id=OIP.9Sx-6uNBXCHu2Ge1fQzeCgHaE7&pid=Api&P=0&w=242&h=162'
        /// Το αλλάζεις με τα δικά σου θέλω

         
const saydark = new Discord.MessageEmbed()
//// Εδώ καθορίζουμε με μορφ΄η Embed το μήνυμα που θα στέλνει το Bot μας.
    .setAuthor(guildname , guild)
    .setColor("BLACK")
    .setTimestamp()  
    .setDescription(message.content)
message.channel.send()
//// Εδώ θα επιστρέψει το Embed μας στο DarkChat κανάλι!
    
      //// Άμα θέλουμε να κάνουμε το μήνυμα να στέλνετε σε απλή μορφή τότε μπορο΄υμε να κάνουμε ενα 
     //// message.channel.send('message.content')
    //// Αλλα είναι ποιο όμορφο εμφανισιακά το Embed!
   
      
      //// Ναι αλλα θα μου πείς δεν δουλε΄υει ετσι και δεν έχει καν Logs!
     //// ναι το γνωρίζουμε δεν θα τα έχεις όλα στο πιάτο εδώ να σε δω πρεπει να βρεις τι δεν έχουμε προστέσει!
  }})
