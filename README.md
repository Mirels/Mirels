### Hi there 👋
MEVCUTBAKİYE = 3000


print("BANKAMIZA HOŞGELDİNİZ ")
print("1-BAKİYE SORGULAMA")
print("2-PARA ÇEKME")
print("3-PARA YATIRMA")
print("a-ÇIKIŞ")



while True:
    İŞLEM = input("LÜTFEN GERÇEKLEŞTİRMEK İSTEDİĞİNİZ İŞLEMİ BELİRLEYİNİZ:")

    if İŞLEM == "a":
        print("ÇIKIŞ İŞLEMİNİZ GERÇEKLEŞTİRİLİYOR LÜTFEN BEKLEYİNİZ....")
        break
    elif İŞLEM == "1":
        print("Bakiyeniz: {}".format(MEVCUTBAKİYE))

    elif İŞLEM=="2":
        TUTAR = int(input ("Lütfen çekmek istediğiniz miktarı giriniz:"))
        if MEVCUTBAKİYE - TUTAR < 0:
            print("ÇEKİLECEK TUTAR MEVCUT BAKİYENİZİN ÜSTÜNDE...")
            continue
        MEVCUTBAKİYE -= TUTAR
        print(f"Bakiyeniz: {MEVCUTBAKİYE}")

    elif İŞLEM == "3":
        TUTAR = int(input ("Lütfen yatırılacak tutarı giriniz:"))

        MEVCUTBAKİYE = MEVCUTBAKİYE + TUTAR
        print("Bakiyeniz: {}".format(MEVCUTBAKİYE))
    else:
        print("Lütfen tekrar deneyiniz!")


