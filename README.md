# Bu kodu kullanmadan önce kütüphaneyi yüklemelisiniz
# pip install instabot

from instabot import Bot

# Botu başlat
bot = Bot()

# Giriş yap
bot.login(username='kullanici_adi', password='sifre')

# Takipçi sayısını öğren
user_info = bot.get_user_info('kullanici_adi')
followers_count = user_info['follower_count']
print(f"Takipçi Sayısı: {followers_count}")
