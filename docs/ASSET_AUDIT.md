# 整理時の確認結果

## 修正した点

- `assets/minecraft/sounds/custom/` を `assets/minecraft/sounds/anlineworld/` に再編。
- 大文字混じりの音源名を小文字・アンダースコアへ統一。
- 未登録だった `dungeon_0_0_0.ogg`、`huenowarutu.ogg`、6本のMP3を、再利用しやすいライブラリBGMとして登録。
- MP3 6本を OGG/Vorbis に変換。Minecraftのリソースパックで再生できる形式に統一。
- `bgm.dungeon.peritune_1` は、元の参照先が存在しなかったため、同梱されていた `dungeon_0_0_0.ogg` を暫定的に割り当て。

## 元パックにあったが音源が不足していたID

以下は参照先の音源ファイルが同梱されていなかったため、整理版の `sounds.json` から外しています。音源を追加したら、対応するIDを登録してください。

- `area.fkd.main.noon` → `custom/environment/fkd/area.fkd.main.noon.ogg` が未同梱
- `area.fkd.castel.library` → `custom/environment/fkd/castel/fkd_castel_library.ogg` が未同梱
- `bgm.system.peakychm` → `custom/system/chm.ogg` が未同梱

## 元MP3

変換前のMP3は別添の `ANLINEWORLD.BGMPACK_original_mp3_sources.zip` に保管しています。
