# ブルートフォース対策

ブルートフォースは攻撃者にとってとても簡単な方法です。General Security chapterで説明したとおり、ブルートフォース対策は、強力なパスワードを設定することです。それとは別に、追加の保護をCAPTCHAで付け足すことができます。

Brute-forcing is theeasy way in for an attacker. General Security chapter, a prerequisite for preventing bruteforcing is to have strong passwords. Apart from that, an additional layer of protection can be added in the form of CAPTCHA.

One good plugin candidate is Google Captcha (reCAPTCHA). The advantage of this plugin is that it can be used to add the extra layer of protection on other areas as well (like registration and comments).

CAPTCHA is not a perfect solution by any means. There are services offering real-time CAPTCHA solving for a few cents per challenge. However it takes seconds to solve a CAPTCHA even for a good service like this, thus this sort of attack becomes unfeasible.

Another preventive measure is to lock-out accounts after a series of failed attempts. There is no plugin at the moment that can lock a user after several failed attempts for a period of time, there are plugins blocking IP addresses that are brute-forcing the login mechanism. This approach is not the best when dealing with distributed attacks.
