Fetching internet data

    #
    # Cet outils fait une simple recherche pour quelquechose sur une cible
    #
    
    import urllib.request
    
    global cible
    cible = "www.rtfm.com"
    quelquechose = "flag"
    
    def main():
        httpurl = urllib.request.urlopen("http://" + cible)
        httpsurl = usllib.request.urlopen("https://" + cible)
        print("HTTP : " + str(httpurl.getcode())
        print("HTTPS : " + str(httpsurl.getcode()))
        httpdata = httpurl.read()
        httpsdata = httpsurl.read()

    if __name__ == "__main__":
      main()
      
 
