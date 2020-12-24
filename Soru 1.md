# Soru 1) 1980’den itibaren spor grubu bazında en çok madalya alan 1. 3. 5. ülkeyi bulalım.

---

```SQL
select Country, count(1) as madalya_sayisi
from sample.summer_medals 
where Year >= 1980
group by Country
order by madalya_sayisi desc
```


| Satır | Country       | madalya_sayisi |
| ------|---------------| --------------:|
| 1     | United States |           1837 |
| 2     | Australia     |            774 |
| 3     | Soviet Union  |            736 |
| 4     | Germany       |            691 |
| 5     | China         |            679 |


**Tabloya göre 1980'den beri en çok madalya alan ülkeler:**
1. ülke `1837` madalya ile `United States`
3. ülke `736` madalya ile `Soviet Union`
5. ülke `679` madalya ile `China` 
