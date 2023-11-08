```mermaid

graph LR;

    goto_bank["銀行でお金をおろす作業時間10分"]

    goto_super["スーパーで卵を買う作業時間10分"]

    wash_egg["卵を洗う作業時間10分"]

    boil_hotwater["お湯を沸かす作業時間20分"]

    boil_eggs["卵をゆでる作業時間10分"]

    crack_the_shell["殻をわる作業時間10分"]

    sprinkle_wit_salt["塩を振る作業時間10分"]

    do_situps["腹筋して腹を減らす作業時間30分"]



subgraph "taro"

 direction LR

 goto_bank--->goto_super--->wash_egg;


   do_situps

end


subgraph "hanako"

 boil_hotwater===>boil_eggs===>crack_the_shell===>sprinkle_wit_salt;

end


 wash_egg--> boil_eggs


```