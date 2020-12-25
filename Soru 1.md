# Soru 1) 1980’den itibaren spor grubu bazında en çok madalya alan 1. 3. 5. ülkeyi bulalım.

---

```SQL
select Country, event, count(1) as madalya_sayisi
from sample.summer_medals 
where Year >= 1980
group by Country, event
order by madalya_sayisi desc
```


| Satır | Country       | event      | madalya_sayisi |
| ------|---------------| -----------|--------------: |
| 1     | United States | basketball |            168 |
| 2     | Netherlands   | hockey     |            159 |
| 3     | Australia     | hockey     |            129 |
| 4     | Cuba          | baseball   |            111 |
| 5     | Brazil        | football   |            109 |


**Tabloya göre 1980'den beri spor grubu bazında en çok madalya alan ülkeler:**
1. ülke `168` madalya ile `basketball` kategorisinde `United States`
3. ülke `129` madalya ile `hockey` kategorisinde `Australia`
5. ülke `109` madalya ile `football` kategorisinde `Brazil` 

