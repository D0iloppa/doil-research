# doil-research

범용 [Claude Code](https://claude.com/claude-code) 스킬. 다중 출처 심층 리서치를
**오케스트레이션**(Opus 계획·판단 / Sonnet 서브에이전트 크롤링), **raw-first 수집**,
**순차·세션간 이어받기**(핸드오프 md) 방식으로 수행한다. 특정 도메인 인프라에 의존하지 않는다.

- 방법론 본문: [`SKILL.md`](SKILL.md)
- 핸드오프 원장 템플릿: [`references/handoff-template.md`](references/handoff-template.md)
- 워크드 예시: [`references/example-rnd.md`](references/example-rnd.md)

## 설치 (글로벌)

개인 Claude Code 스킬 디렉토리로 링크하면 어디서든 트리거된다.

```bash
git clone https://github.com/D0iloppa/doil-research.git
cd doil-research
./install.sh          # 이 스킬을 <config>/skills/ 로 심볼릭 링크
```

`install.sh`는 `CLAUDE_CONFIG_DIR`(없으면 `~/.claude`)의 `skills/`에 이 repo를 링크한다.

여러 스킬을 함께 관리하려면 집계 repo [`D0iloppa/skills`](https://github.com/D0iloppa/skills)가
이 repo를 서브모듈로 장착한다.
