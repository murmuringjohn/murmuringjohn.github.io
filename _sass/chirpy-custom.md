

    /* 1. 메인 화면의 글 목록(Post List) 스타일 설정 */
    #post-list {
      /* 글 제목 스타일 */
      .post-preview {
        h1 {
          font-size: 1.6rem;       /* 기존보다 명확하게 키우거나 조절 (기본값은 보통 1.4~1.5rem) */
          font-weight: 700;        /* 제목을 더 두껍게 하여 강조 */
          line-height: 1.3;
          margin-bottom: 0.5rem;
        }
    /* 글 요약/설명(Description) 스타일 */
    .post-content {
      p {
        font-size: 1.0rem;     /* 제목과 확연히 구분되도록 크기 조절 */
        font-weight: 400;      /* 본문은 가볍게 */
        color: var(--text-muted); /* 회색 톤으로 대비 부여 */
        line-height: 1.5;
           }
         }
      }
    }
    
    /* 2. 모바일 반응형 대응 (필요시 조절) */
    @include media-breakpoint-down(md) {
      #post-list {
        .post-preview {
          h1 {
            font-size: 1.4rem;
          }
          .post-content {
            p {
              font-size: 0.95rem;
            }
          }
        }
      }
    }
    
    /* 기존에 만드신 본문용 코드도 유지하고 싶다면 아래에 그대로 두시면 됩니다 */
    .post-title {
      font-size: 2.3rem;
      line-height: 1.25;
    }
    .post-subtitle,
    .post-description {
      font-size: 1.18rem;
      margin-top: 0.6rem;
      font-weight: 400;
      color: var(--text-muted);
    }