# Documentacao Senai-Ibge
# Desenvolvimento de Sistemas 
# Aluno: Pedro Henrique Lemos Santos 


**tag KeyboardAvoidingView**

|Utilizado para impedir que o teclado cubra o texto que aparece na tela, impedindo que a visibilidade do usuário seja perdida

|Vídeo youtube: https://www.youtube.com/watch?v=JTpZ81k2wiE

|Código:  <KeyboardAvoidingView style={Style.container}>

**tag view**

|Utilizado para a criação da interface, onde ele referencia outros comandos, como no exemplo abaixo

|Vídeo youtube: https://www.youtube.com/watch?v=Xpg2x1ZZ9co

|Código: <View style={Style.body}>

**tag text**

|Utilizado para mostrar na interface mensagens ou qualquer tipo de texto

|Vídeo youtube: https://www.youtube.com/watch?v=_YydVvnjNFE

|Código:  <Text style={Style.textHeader}>{welcome}</Text>

**tag textinput**

|Espaço reservado para que o usuário digite agluma informação dele ou alguma informação necessária para a utilização do sistema

|Vídeo youtube: https://www.youtube.com/watch?v=c9Sg9jDitm8

|Código: <TextInput placeholder='Digite seu nome (Sem espaço)' onChangeText={(name) => { setName(name); }} placeholderTextColor='#fff' style={Style.input} />

**tag Toucheableopacity**

|Utilizada para controlar a opacidade

|Vídeo youtube: https://www.youtube.com/watch?v=cGZuXWffGEM

|Código: <TouchableOpacity style={Style.button} onPress={() => { SearchController(name, year, navigation); }}><Text style={Style.buttonText}>Exibir</Text></TouchableOpacity>

**tag logo**

|Seria a tag image

|Foi criada nesse sistema, para utilizarmos a logo do senai

|Vídeo youtube: https://www.youtube.com/watch?v=v-3sNvMNosY

|Código: <Logo style={{ fillRule: 'evenodd', width: '75%', height: '25%', alignItems: 'center' }} />


# Documentação Senai-Corona
# Desenvolvimento de Sistemas

**tag container**

|Objeto que contém outros objetos que podem ser excluídos e incluídos 

|Vídeo youtube: https://www.youtube.com/watch?v=m2q3Dyr6To4

|Código: <Container>
      <StatusBar barStyle="light-content" backgroundColor="#0f7778" />
      <Header> 
      ...
        </Container>


**tag statusbar**

|Responsável pela barra de status do programa, ou seja, controla ela

|Vídeo youtube: https://www.youtube.com/watch?v=J1nfPQGr21c

|Código: <StatusBar barStyle="light-content" backgroundColor="#0f7778" />

**tag header**

|São cabeçalhos onde ficam as informações e ações relacionadas a tela atual

|Vídeo youtube: https://www.youtube.com/watch?v=C3oDJdlrEKE

|Código: <Header>
        <TextHeader>COVID - 19</TextHeader>
        <ImageHeader source={logoImg} />
         </Header>

**tag textheader**

|É utilizado para adicionar o texto que vai aparecer no cabeçalho

|Vídeo youtube: Não encontrado

|Código:  <Header>
        <TextHeader>COVID - 19</TextHeader>
        <ImageHeader source={logoImg} />
         </Header>

**tag imageheader**

|É utilizado para adicionar imagem no cabeçalho

|Vídeo youtube: Não encontrado, mas vou deixar um vídeo com outras formas de adicionar imagem https://www.youtube.com/watch?v=SSJc6ZUo5HI

|Código: <Header>
        <TextHeader>COVID - 19</TextHeader>
        <ImageHeader source={logoImg} />
         </Header>

**tag mapview**

|Permite a visualização do mapa

|Vídeo youtube: https://www.youtube.com/watch?v=AzjWv1X-uyg

|Código: <MapView
        onRegionChangeComplete={handleRegionChanged}
        style={{ flex: 1 }}
        initialRegion={region}
        >
        </MapVie>
        ...

**tag marker**

|É o marcador do mapa

|Vídeo youtube: https://www.youtube.com/watch?v=WKS8cCbnyHQ

|Código: <Marker
              key={state.uf}
              coordinate={{
                latitude: Number(state.latitude),
                longitude: Number(state.longitude),
              }}
            >

**tag imagemarker**

|Utilizado para selecionar imagem do mapa

|Vídeo youtube: https://www.youtube.com/watch?v=AzjWv1X-uyg

|Código: <ImageMarker source={logoImg} />

**tag callout**

|Está chamando as informações de casos em cada estado

|Vídeo youtube: https://www.youtube.com/watch?v=4N-8RTeQ1fA

|Código: <Callout>
                <CalloutContent>
                  <CalloutText>{state.state}</CalloutText>
                  ...

**tag calloutcontent**

|Mostrar as informações 

|Vídeo youtube: Não encontrado

|Código: <Callout>
                <CalloutContent>
                  <CalloutText>{state.state}</CalloutText>
                  ...

**tag callouttext**

|Onde vai aparecer as informações de mortos, infectados etc

|Vídeo youtube: https://www.youtube.com/watch?v=WKS8cCbnyHQ

|Código: <CalloutText>{state.state}</CalloutText>
                  <CalloutText>Casos Confirmados: {state.cases}</CalloutText>
                  <CalloutText>Mortos: {state.deaths}</CalloutText>
                  <CalloutText>


# Documentação Senaiflix
# Desenvolvimento de Sistemas

**tag view**

|Utilizado para a criação da interface, onde ele referencia outros comandos, como no exemplo abaixo

|Vídeo youtube: https://www.youtube.com/watch?v=Xpg2x1ZZ9co

|Código:<View style={Styles.body}>

**tag text**

|Utilizado para mostrar na interface mensagens ou qualquer tipo de texto

|Vídeo youtube: https://www.youtube.com/watch?v=_YydVvnjNFE

|Código: <Text style={Styles.title}>Disciplinas</Text>

**tag Toucheableopacity**

|Utilizada para controlar a opacidade

|Vídeo youtube: https://www.youtube.com/watch?v=cGZuXWffGEM

|Código: <TouchableOpacity onPress={() => { navigation.navigate('Playlist', { id: item.id }); }} style={Styles.categoryButton}>
                        <Text style={Styles.titleButtonCategory}>{ item.name }</Text>
                    </TouchableOpacity>

**tag image**

|Utilizada para adicionar imagem no programa

|Vídeo youtube: https://www.youtube.com/watch?v=SSJc6ZUo5HI

|Código:  <Image source={Logo} style={Styles.logo} />

**tag flatlist**

|Utilizado para criar e redenrizar listas

|Vídeo youtube: https://www.youtube.com/watch?v=zjAU6QeEGGg

|Código: <FlatList style={Styles.list} data={subjects} keyExtractor={subject => subject.id} renderItem={({ item }) => {
                return (

**tag webview**

|Utilizado para exibir conteúdo da web

|Vídeo youtube: https://www.youtube.com/watch?v=q4o5xgRALms

|Código: <WebView source={{ uri: videoURL }} allowsFullscreenVideo={true} />


# Documentação Senai
# Desenvolvimento de Sistemas

**tag view**

|Utilizado para a criação da interface, onde ele referencia outros comandos, como no exemplo abaixo

|Vídeo youtube: https://www.youtube.com/watch?v=Xpg2x1ZZ9co

|Código: <View style={styles.header}>
                <Image source={logoImg} />
                <TouchableOpacity onPress={navigationBack}>
                    <Feather name="arrow-left" size={28} color="#E82041" />
                </TouchableOpacity>
            </View>

**tag text**

|Utilizado para mostrar na interface mensagens ou qualquer tipo de texto

|Vídeo youtube: https://www.youtube.com/watch?v=_YydVvnjNFE

|Código:  <Text style={[styles.incidentProperty, {marginTop:0}]}>ONG:</Text>

**tag feather**

|

|Vídeo youtube: https://www.youtube.com/watch?v=l2OIBV4RfAU

|Código:  <Feather name="arrow-left" size={28} color="#E82041" />

**tag Toucheableopacity**

|Utilizada para controlar a opacidade

|Vídeo youtube: https://www.youtube.com/watch?v=cGZuXWffGEM

|Código: <TouchableOpacity style={styles.action} onPress = {sendMail}>
                        <Text style={styles.actionText}>E-mail</Text>
                    </TouchableOpacity>
